---
layout: default
title: "Privacy Policy"
nav_order: 2
---

# Privacy Policy

**Effective date:** 2026-08-05
**Applies to:** Open Perch for iOS, version 0.1.0 and later

---

## The short version

Open Perch is an offline-first birding app. Read this bit and you have the gist:

- **We have no servers and no accounts.** There is nowhere for us to send your data, because we do not operate a backend.
- **Your sightings, notes, and locations stay on your phone.** They live in a database on the device and are deleted when you delete the app.
- **Sound identification runs entirely on your device.** Audio is analyzed in memory, is never written to storage, and is never uploaded.
- **We collect no analytics, no advertising identifiers, and no crash telemetry.** We genuinely do not know how many people use this app or what they do in it.
- **Two things do leave your device, and only when you ask for them:** looking up a place name for a sighting, and loading map tiles. Both go to OpenStreetMap. Details below — we would rather over-explain this than let you find it out yourself.

That's the whole policy in spirit. The rest is the precise version.

---

## 1. Who we are

Open Perch is maintained by Miadad Rashid. You can reach us at **support@openperch.org** about anything in this document.

## 2. What the app stores, and where

Everything below is stored **only in the app's private storage on your device**. None of it is transmitted to us — we have no service to transmit it to.

| What | Why it exists | Where it lives |
|---|---|---|
| Observations (species, date and time, optional notes) | The point of the app — your personal sightings log | On-device database |
| Coordinates attached to an observation, if you add one | Shows sightings on your map and sorts your life list | On-device database |
| A place label for those coordinates (e.g. "Travis County, Texas") | Makes the sightings list readable | On-device database |
| Your chosen location precision (exact, ~1 km, or town-level) | Applies your privacy preference to what gets recorded | On-device database |
| App settings | Remembers your preferences | On-device storage |

**Deleting the app deletes all of it.** We cannot recover it for you, and there is no backup on our side, because there is no our side. If your device backs itself up to iCloud, the app's data may be included in that backup under Apple's terms — that is between you and Apple, and we have no access to it.

## 3. Location

Location is **optional**. The app works without it, and you can log sightings with no location at all.

When you attach a location:

- The app asks iOS for your coordinates using the standard system permission. iOS shows you the prompt, and you can refuse or revoke it any time in Settings.
- You choose how precisely the location is recorded: **exact**, **approximately 1 km**, or **town level**. If you choose a coarser setting, the coordinates are rounded *before* they are stored — the precise position is discarded, not merely hidden.
- The result is saved on your device and nowhere else.

**We never use location for advertising, profiling, or tracking, and we never share it.** We could not share it if we wanted to; it never reaches us.

## 4. The microphone and sound identification

Open Perch can listen to a bird call and suggest which species it might be.

- The microphone is active **only** while the Listen screen is open and you have tapped the record control. It stops when you stop, leave the screen, or close the app.
- Audio is processed **entirely on your device** by a bundled machine-learning model. It is held briefly in memory in short segments and then discarded.
- **Recordings are never saved to storage and never leave the device.** There is no upload, no cloud analysis, and no network request involved in identification. It works in airplane mode, which is a useful way to verify this claim for yourself.
- The identification model is BirdNET, developed by the Cornell Lab of Ornithology and Chemnitz University of Technology, licensed CC BY-NC-SA 4.0. The model is embedded in the app and runs locally; using it sends nothing to Cornell or anyone else.

## 5. What does leave your device

Two features make outbound network requests. Both are to **OpenStreetMap**, a non-profit mapping project, and both happen only in response to something you do.

**Place-name lookup (Nominatim).** When you attach a location to a sighting, or search for a place by name, the app sends a request to `nominatim.openstreetmap.org`:

- For a location you captured, the request contains **the coordinates** so OpenStreetMap can return a human-readable place name.
- For a place search, the request contains **the text you typed**.
- The request identifies the app and version and includes a link to our public issue tracker, as OpenStreetMap's usage policy requires. It contains no account identifier, no device identifier, and no name or email of yours.
- Results are cached in memory so repeating the same lookup does not repeat the request.

Note that if you have chosen a coarser location precision, the coarsened coordinates are what get sent.

**Map tiles.** The map view loads map imagery from `tile.openstreetmap.org`. As with any online map, the tiles requested reveal **which area of the map you are looking at** to the tile server. This is inherent to how online maps work, not something specific to Open Perch. If you never open the map view, no tiles are requested.

Both services are operated by the OpenStreetMap Foundation under their own privacy policy, which we do not control: <https://wiki.osmfoundation.org/wiki/Privacy_Policy>. Like any web request, these carry your IP address to OpenStreetMap's servers.

**That is the complete list.** There are no other outbound connections in the app.

## 6. What we do not do

To be explicit, because plenty of apps do these things:

- No analytics or usage tracking of any kind
- No advertising, ad networks, or advertising identifiers
- No crash or performance telemetry
- No third-party SDKs that collect data
- No accounts, logins, or email collection
- No selling, renting, or sharing of personal information — we hold none to sell
- No tracking across apps or websites, as Apple's App Tracking Transparency framework defines it

## 7. Children

Open Perch is suitable for all ages and does not knowingly collect personal information from anyone, children included. There are no accounts and no user-to-user contact.

## 8. Your rights

Because your data is on your device and under your control:

- **Access it** — everything is visible in the app.
- **Correct it** — edit or delete any observation directly.
- **Delete all of it** — delete individual observations, or remove the app to erase everything.
- **Withdraw permissions** — revoke location or microphone access in iOS Settings at any time. The rest of the app keeps working.

We cannot action a data access or deletion request on your behalf for the simple reason that we hold no copy of your data. If you are in a jurisdiction granting you rights under the GDPR, the CCPA, or similar law, those rights are satisfied by the controls above; write to us at support@openperch.org if something is unclear and we will explain it properly.

## 9. Changes to this policy

Open Perch is in active development, and a future version is planned to add optional community features that would sync data to a server. **That would be a material change to this policy.** If and when it happens:

- This policy will be updated with a new effective date.
- The app will tell you about the change in-app before any new data practice takes effect.
- Anything that involves sending your data off the device will be **opt-in**. It will not be switched on for you.

Until you see such a notice, the policy you are reading is the one in force.

## 10. Contact

Questions, corrections, or concerns: **support@openperch.org**

You can also open a public issue at https://github.com/miadadrashid/open-perch-site/issues.
