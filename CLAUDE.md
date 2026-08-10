# KNX — HOS Approaching Limit Add-In

## Goal
Standalone MyGeotab page add-in for Knight Transportation showing drivers with < 1 hour of drive time remaining who are currently on-duty or driving.

## Key Info
- **Customer:** Knight Transportation (`knight_transportation_prod`)
- **CompanyGuid:** `f5d09ffc-cdec-428c-b30e-68fd02985383`
- **Data source:** `DutyStatusAvailability` API object (fields: `driving`, `duty`, `rest`, `workday`, `cycle` remaining durations)
- **Reference report:** `https://my.geotab.com/knight_transportation_prod/#customReport,id:bA2,scheduleId:bB8,source:HosAvailability,type:dashboard`

## Spec
- Threshold: < 1 hour remaining drive time (configurable)
- Filter: on-duty / driving drivers only (configurable)
- Display: color-coded table (red/yellow/green), auto-refreshing
- Type: standalone page add-in (not a button add-in)

## Files
- `index.html` — main add-in entry point
- `addin.json` — add-in configuration for MyGeotab
- `README.md` — deployment instructions

## Status
In progress.
