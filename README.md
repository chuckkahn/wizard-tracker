# eBay Wizard Tracker

A crowdsourced archive of eBay Wizard sightings from Fan Expo Canada 2026 in the Metro Toronto Convention Centre.

Live site:  
https://chuckkahn.github.io/wizard-tracker/

## How it works

1. Select an event day to explore its sightings.
2. Select the MTCC level where a wizard was spotted.
3. Tap the historical location on the floor plan.
4. Choose the wizard colour:
   - Red
   - Blue
   - Yellow
   - Green
5. Enter the Toronto date and time from Thursday, August 27 through Sunday, August 30, 2026.
6. Optionally add your name or social handle.
7. Add the historical sighting.

Each event day has its own view. Lines connect successive sightings of the same wizard colour on the same level in chronological order.

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

Sightings are shared between visitors through Supabase. New entries are restricted to the four Fan Expo event dates. The browser also keeps a local cache and queues submissions made while cloud sync is unavailable, retrying them when the connection returns.

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
