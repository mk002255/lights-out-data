# Lights Out — Remote Data

Remote config source for the [Lights Out](https://github.com/mk002255) F1 companion app.

Team staff and driver bio data live here as JSON, fetched by the app at launch so
personnel/roster corrections don't require a new App Store build.

## Files

- `teams.json` — per-constructor data (team principal, chief engineer, race engineer pairings, history, career stats)
- `drivers.json` — per-driver data (bio, nationality, DOB, career stats)

## Editing

Edit a file directly on github.com (pencil icon → change value → commit).
The app fetches the raw file, so a commit to `main` takes effect next app launch.

Keep the JSON keys and structure as-is — the app expects the same shape as
`TeamHistory`/`DriverBio` in the Swift source.
