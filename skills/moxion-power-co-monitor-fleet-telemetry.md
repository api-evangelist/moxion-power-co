---
name: Monitor Moxion Mobile Power Unit fleet telemetry
description: >-
  Authenticate to the Moxion Power Developer API and pull an organization's
  Mobile Power Units, their latest location, recent metrics, and any active
  faults — the core fleet-monitoring flow.
api: openapi/moxion-power-co-openapi.yml
operations:
  - OrganizationsController_listOrganizations
  - DevicesController_listDevices
  - DevicesController_getDevice
  - DeviceLocationController_getLatestLocation
  - DeviceMetricsController_listMetrics
  - DeviceFaultsController_listFaults
  - FleetFaultSnapshotController_listEquipmentAempFaultSnapshot
---

# Monitor Moxion Mobile Power Unit fleet telemetry

Read-only flow over the Moxion Power Developer API (`http://api.moxionpower.com/developer/v1`).

## Auth
Send every request with an API key issued to a Service Account:
`Authorization: bearer <TOKEN>`. Service Accounts and their permissions are
provisioned by Moxion personnel (see `authentication/moxion-power-co-authentication.yml`).

## Steps
1. **Confirm scope** — call `OrganizationsController_listOrganizations` to list the
   organizations the token is authorized for.
2. **List the fleet** — call `DevicesController_listDevices` to enumerate the
   organization's Mobile Power Units; optionally `DevicesController_getDevice`
   for a single device's details.
3. **Locate a device** — call `DeviceLocationController_getLatestLocation` for the
   current position (or `DeviceLocationController_listLocations` for history).
4. **Pull recent metrics** — call `DeviceMetricsController_listMetrics` with
   `start`/`end`. The range is half-open `[start, end)` and may not exceed **1 day**;
   page backwards a day at a time for longer windows. Metric names/units are in
   `vocabulary/moxion-power-co-metrics.yml` (e.g. `pack.soc`, `pack.power_net`).
5. **Check for faults** — call `DeviceFaultsController_listFaults` per device, or
   `FleetFaultSnapshotController_listEquipmentAempFaultSnapshot` for the whole fleet
   at once. Only **ACTIVE** faults are returned; a zero-length array means none known.
   Map fault codes and `CRITICAL`/`INFO` severity via `errors/moxion-power-co-fault-codes.yml`.

## Conventions & errors
- Time-range endpoints require `start` and `end` (ISO 8601); max duration 1 day.
- On HTTP **429** you have exceeded the request rate limit or the data-row quota —
  back off and retry. See `conventions/moxion-power-co-conventions.yml`.
- `401` means a missing/invalid bearer token; `404` an unknown device.
