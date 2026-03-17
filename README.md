# NYU Bus Tracker

A simple mobile-first web app for tracking NYU shuttle bus schedules with real-time countdown timers.

![NYU Bus Tracker](images/nyu_logo.png)

## Features

- Real-time countdown to the next bus at each stop
- Schedules for all 7 NYU shuttle routes (A, B, C, E, F, G, W)
- Day-aware scheduling — automatically loads the correct schedule for weekdays, Fridays, and weekends
- Route map images for each line
- Live status indicator showing how many routes are running today
- Dark theme UI designed to feel like a native mobile app
- On desktop, renders as a centered phone-sized container

## Routes

| Route | Color | Area |
|-------|-------|------|
| A | Purple | Brooklyn / MetroTech |
| B | Blue | SoHo / Greenwich Village |
| C | Green | Stuyvesant Town |
| E | Orange | Langone / Gramercy |
| F | Pink | Kips Bay |
| G | Teal | West Village |
| W | Brown | Weekend Downtown |

## Project Structure

```
NYU_BUS_Web_App/
├── index.html          # Entire app — HTML, CSS, and JS in one file
├── data/               # JSON schedule files (per route × day type)
│   ├── Route_A_Schedule_Monday-Thursday.json
│   ├── Route_A_Schedule_Friday.json
│   ├── Route_A_Schedule_Weekend.json
│   └── ...
└── images/             # Route map images and logos
    ├── apic.png        # Route A map
    ├── bpic.png        # Route B map
    └── ...
```

## Tech Stack

- Vanilla HTML, CSS, and JavaScript — no frameworks or dependencies
- Schedule data stored as static JSON files
- Single-file architecture (`index.html`)
