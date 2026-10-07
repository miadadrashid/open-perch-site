---
layout: default
title: "Open Perch — Help & Support"
nav_order: 1
---

# Open Perch — Help & Support

Open Perch is an offline-first birding app for iOS: a species guide, a personal sightings log, a map of where you have been, and on-device identification of bird calls.

## Contact

**support@openperch.org**

It's a small project, so replies come from a person rather than a helpdesk. Expect a few days.

When reporting a problem, these help enormously:

- Your iPhone model and iOS version
- What you did, what you expected, what happened instead
- A screenshot if the problem is visible

You can also open a public issue at https://github.com/miadadrashid/open-perch-site/issues.

---

## Frequently asked

### Does Open Perch work without a signal?

Yes — that's the point of it. The species guide, your sightings log, and sound identification all work fully offline. Only two things need a connection: looking up the name of a place, and loading map imagery. Everything else works in the middle of nowhere, which is where the birds are.

### Where is my data stored? Can you see it?

On your phone, and no. There are no accounts and no servers. Your sightings never reach us. See the [Privacy Policy](https://help.openperch.org/privacy) for the full detail, including the two requests that do go out to OpenStreetMap.

### How accurate is sound identification?

It's a suggestion, not an answer. The app uses BirdNET, a well-regarded model from the Cornell Lab of Ornithology, running entirely on your phone. It does well with a clear, close call and struggles with wind, distance, traffic, and several birds calling at once. Treat a result as a strong hint, and confirm it yourself before adding a lifer.

That's also why results are labelled "possible match" rather than presented as fact.

### Why did it identify a bird that isn't in the app's guide?

The identification model knows about 6,500 species worldwide. The current species guide carries a much smaller curated set. When the model recognizes something outside that set, you'll see the name but no guide entry to open and no way to log it yet. The guide is being expanded.

### Why does it need the microphone?

Only to listen for bird calls, and only while the Listen screen is open and you've started it. Audio is analyzed on your device and never saved or uploaded. You can decline the permission and use the rest of the app normally.

### Can I control how precisely my locations are recorded?

Yes. Each sighting can be recorded at exact, roughly 1 km, or town-level precision. Coarser settings round the coordinates *before* saving — the exact position is discarded rather than hidden.

### How do I delete my data?

Delete individual sightings in the app, or delete the app to erase everything at once. Note that if your iPhone backs up to iCloud, app data may be included in that backup under Apple's terms.

### Is my life list backed up?

Not by us. It lives on your device. An iCloud device backup may include it, but there is no Open Perch account to restore from. Treat your sightings as device-local for now.

---

## Known issues

None recorded for the initial release. Problems found after launch will be listed here.

---

## Legal

- [Privacy Policy](https://help.openperch.org/privacy)
- [Terms of Service](https://help.openperch.org/terms)

Bird identification powered by BirdNET (Cornell Lab of Ornithology and Chemnitz University of Technology), licensed CC BY-NC-SA 4.0. Map data and place names © OpenStreetMap contributors.
