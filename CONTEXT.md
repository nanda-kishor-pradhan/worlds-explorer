# Worlds Explorer — Project Context

## Vision
Ek minimal, immersive, open source 3D globe-based web explorer
jisme user Earth, Mars, Moon, Ocean Floor, aur Prehistoric Earth
explore kar sake — sab ek hi place pe. Google Street View jaisi
feel but entire worlds ke liye.

---

## Tech Stack
- Frontend: React + Vite
- 3D Engine: CesiumJS
- Styling: TailwindCSS
- Hosting: GitHub Pages / Vercel
- APIs: NASA, NOAA, USGS, OpenWeatherMap, 
        WAQI, Wikipedia REST, Wikimedia Commons,
        OpenStreetMap Nominatim (sab free)

---

## Design Rules
1. "Agar element hata do aur fark na pade — hata do."
2. Globe = hero. UI = supporting cast.
3. Minimal interactions, maximum immersion.
4. No login. No ads. No clutter.

## Color Palette
- Background:  #0A0A0F
- Surface:     #111118
- Accent:      #4A9EFF
- Text:        #E8E8F0
- Muted:       #555566

---

## UI Layout

### Landing Screen
- Dark space background
- Earth slowly rotating
- "WORLDS EXPLORER" text
- Single [ Enter ] button
- Koi extra text nahi

### Main Explorer Screen
- Top bar: Logo + Search icon + Menu (minimal)
- 92% screen: 3D Globe
- Floating right: Bookmark, Cinematic, Random Explore buttons
- Bottom strip: World switcher
  🌍 Earth | 🔴 Mars | 🌙 Moon | 🌊 Ocean | 🦕 Prehistoric | ⏱️ Compare

### Search Bar (click to expand)
- Recent searches
- Discover suggestions (curated interesting locations)
- Works across all worlds

### Info Panel (right side, slide in on click)
- Triggered by: clicking any location on globe
- Content varies by what was clicked:
  - Mountain: Name, Height, Range, First Climbed, Coordinates
  - City: Name, Population, Country, Timezone, Live Weather
  - Ocean: Depth, Temperature, Nearest Trench
  - Mars Crater: Name, Diameter, Age, NASA Photos
  - Random area: Lat/Long, Region, Nearest Landmark
- Always includes: Wikipedia snippet, Wikimedia photos,
  Save button, Share button
- Close: ESC or X button

### Layers Panel (toggle from top)
- Satellite ON/OFF
- Terrain ON/OFF
- Weather ON/OFF
- AQI/Pollution ON/OFF
- Night Lights ON/OFF
- Population Density ON/OFF
- Forest Cover ON/OFF
- Live Disasters ON/OFF

---

## Worlds & Features

### 🌍 Earth
- Real satellite imagery
- Real-time weather overlay
- AQI / pollution layer
- NASA Black Marble night lights
- Population density heatmap
- Forest cover change slider (2000 vs now)
- Real-time sun position (day/night live)
- ISS live tracker
- Live disaster layer (wildfires, earthquakes, hurricanes)

### 🔴 Mars
- NASA Curiosity + Perseverance rover photos
- Named locations (Olympus Mons, Valles Marineris etc)
- Live rover location
- Terrain elevation colors
- Dust storm history overlay

### 🌙 Moon
- Apollo 11, 12 landing sites
- Crater database
- Dark/bright side toggle
- Lunar elevation map

### 🌊 Ocean Floor
- NOAA bathymetry data
- Mariana Trench zoom
- Underwater volcano locations
- Shipwreck markers
- Ocean temperature layer

### 🦕 Prehistoric Earth
- Time slider: 500M BC to present
- Continent drift animation
- Climate overlay per era
- Paleogeography open data

---

## Cross-World Features
- Universal Search (one bar, all worlds)
- Bookmark + Share via URL
  Format: worlds-explorer.vercel.app/mars/olympus-mons
- Cinematic Mode (no UI, globe rotates, screensaver feel)
- Compare Mode (split screen, drag to resize)
- Random Explore ("Surprise Me" button)
- Photo Mode (screenshot with auto watermark)
- Ambient Sound toggle
  - Earth: nature sounds
  - Mars: NASA recorded wind
  - Ocean: underwater sounds
- Space Missions Timeline sidebar
- Mini Map (corner, shows position when zoomed in)
- Wikipedia integration on info panel

---

## Data Sources
- OpenStreetMap Nominatim  →  Location search + names
- Wikipedia REST API       →  Info snippets
- Wikimedia Commons API    →  Free photos
- OpenWeatherMap API       →  Live weather
- WAQI API                 →  AQI data
- NASA APIs                →  Mars, Moon, ISS, Black Marble
- NOAA                     →  Ocean bathymetry
- USGS                     →  Earthquakes, planetary names
- NASA FIRMS               →  Live wildfire data

---

## What We Are NOT Building
- Login / Signup
- Comments section
- Ads
- 3D buildings
- Traffic data
- Mobile app (maybe phase 6)
- Gamification / points system

---

## Development Phases

### Phase 1 — Core Foundation
- React + Vite + CesiumJS setup
- Earth globe with satellite imagery
- Search bar (Earth locations)
- Basic layers toggle
- Info panel (right slide-in)
- Bookmark + Share URL

### Phase 2 — All Worlds
- Mars + Moon + Ocean + Prehistoric
- NASA photo integration
- Time slider for Prehistoric Earth
- World switcher animations

### Phase 3 — Wow Features
- Cinematic Mode
- Ambient Sound
- Live Disaster Layer
- ISS Live Tracker
- Real-time sun position

### Phase 4 — Polish
- Compare Mode
- Photo Mode
- Random Explore
- Space Missions Timeline
- Mini Map
- Wikipedia integration

### Phase 5 — Community
- User photo pins
- Shareable collections

---

## Current Status
Planning complete. Starting Phase 1.
Repo: not created yet.

## Instructions for AI
Read this file fully before starting.
Always follow the design rules.
Ask before adding features not listed here.
Reference PROGRESS.md for current status.
