# eBay Wizard Tracker

A simple crowdsourced map for tracking eBay Wizard sightings at Fan Expo Canada in the Metro Toronto Convention Centre.

Live site:  
https://chuckkahn.github.io/wizard-tracker/

## How it works

1. Select the MTCC level where you spotted a wizard.
2. Tap the location on the floor plan.
3. Choose the wizard colour:
   - Red
   - Blue
   - Yellow
   - Green
4. Optionally add your name or social handle.
5. Log the sighting.

Recent sightings appear on the corresponding floor plan and fade as they get older.

## MTCC levels

### North Building — Front Street
- Level 100
- Level 200
- Level 300

### South Building — Bremner Blvd.
- Level 500
- Level 600
- Level 700
- Level 800

Levels 300 and 800 use the Fan Expo-specific show maps. The other levels use official Metro Toronto Convention Centre floor plans.

## Privacy and storage

Sightings are shared between visitors through Supabase. The browser also keeps a local cache and queues submissions made while cloud sync is unavailable, retrying them when the connection returns.

The public browser key can read and insert sightings only; database permissions should continue to deny updates and deletes for anonymous visitors.

## Project structure

```text
wizard-tracker/
├── index.html
├── maps/
│   ├── mtcc-level-100.png
│   ├── mtcc-level-200.png
│   ├── mtcc-level-500.png
│   ├── mtcc-level-600.png
│   └── mtcc-level-700.png
├── README.md
└── LICENSE
