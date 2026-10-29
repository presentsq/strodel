# Strodel Privacy Policy

Effective date: October 29, 2026

This policy covers the Strodel iOS application ("the app").

## 1. Data processed

**Location.** While a walk is active (from *Hold to start walk* until *Stop*),
the app reads GPS fixes (latitude, longitude, horizontal accuracy, altitude,
timestamp) from iOS Core Location, in the foreground and, if background
location permission is granted, in the background. Fixes are written to a
journal file on the device and used to compute the walked route, the claimed
area, distance and time. Outside an active walk, the current position is used
only to position the map and is not stored.

**Barometric pressure.** If motion permission is granted, the app samples the
barometer during a walk to compute elevation gain. Samples are stored with the
route.

**Game state.** Routes, claimed cells, plots, levels, buildings, currency and
preferences derived from walks.

No account, name, e-mail address, contacts, photos or device identifiers are
collected.

## 2. Storage

All data in section 1 is stored in the app's sandboxed container on the device.
The app operates no server. No data is transmitted to the developer. Deleting
the app deletes the data. iCloud device backups may include the container
according to the user's iOS backup settings.

## 3. Network requests

- **Map tiles.** The app requests vector tiles for the visible map area from
  OpenFreeMap (`tiles.openfreemap.org`), which serves OpenStreetMap data. The
  request discloses the device's IP address and the requested tile coordinates
  to that service. Walk data is not sent. OpenFreeMap's handling of requests is
  governed by its own policy at https://openfreemap.org.
- **TestFlight (beta builds only).** Apple collects crash logs and
  user-submitted feedback under the TestFlight terms.

The app contains no analytics SDK, advertising SDK or tracking. Ads shown in
beta builds are placeholders rendered locally.

## 4. Data sharing initiated by the user

- *Share* on a walk exports that walk's summary through the iOS share sheet.
- *Copy debug info* exports a diagnostic text (app version, device model, recent
  rendering statistics, error messages). It contains no coordinates, routes or
  addresses.

Both actions send data only to the destination the user selects.

## 5. Permissions

| iOS permission | purpose | required |
|---|---|---|
| Location, When In Use | map positioning; walk recording while the app is in the foreground | yes, for walks |
| Location, Always | walk recording while the app is in the background | no |
| Motion & Fitness | barometer sampling for elevation gain | no |

Permissions can be changed in iOS Settings at any time.

## 6. Changes

Changes to this policy are published at this URL with a new effective date.

## 7. Contact

presentsq — presentsq.dev@gmail.com
