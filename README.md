# TTET's Footprint | Interactive Journey Log

A cinematic, interactive web mapping application designed to visualize and replay travel history across Asia, Europe, and beyond. Built with a focus on aesthetics, smooth animations, and an immersive user experience.

## ✨ Features

* **Cinematic Journey Playback:** Animate your travel route step-by-step with great circle flight paths, a moving traveler icon, and adjustable playback speeds (0.5x, 1x, 1.5x, 2x).
* **Atmospheric Visuals:** Includes a toggleable film grain texture and vignette overlay for a moody, cinematic aesthetic.
* **Interactive Map Controls:** 
  * Custom dark-themed Carto basemaps.
  * Fancy pulsing markers for visited locations.
  * Toggleable place labels and journey trails.
* **Advanced Search & Filtering:**
  * Dropdown filter to isolate locations by specific countries.
  * Real-time text search for cities, countries, or specific location details.
* **Responsive & Accessible:** 
  * Fully responsive design optimized for both desktop and mobile devices.
  * Respects `prefers-reduced-motion` OS settings by disabling heavy animations.
  * ARIA labels and screen-reader-friendly DOM structures.

## 🛠️ Technologies Used

* **HTML5 / CSS3:** Native styling with CSS variables, complex keyframe animations, and backdrop filters.
* **Vanilla JavaScript (ES6):** No heavy frameworks; clean, modular logic for state management and DOM manipulation.
* **[Leaflet.js](https://leafletjs.com/):** Open-source JavaScript library for mobile-friendly interactive maps.
* **[Carto](https://carto.com/):** Dark matter map tiles.
* **Fonts:** Montserrat (UI) and Cormorant Garamond (Typography).

## 🚀 Getting Started

Since this project is contained entirely within a single file and relies on CDNs for external libraries, setup is instant.

1. Clone or download the repository.
2. Open `index.html` (or whatever you named the stitched file) directly in any modern web browser.
3. *Optional:* Host it on any static file hosting service (e.g., GitHub Pages, Vercel, Netlify) to share it live.

## 🗺️ Adding New Locations

Travel data is stored directly within the JavaScript script block in a pipe-delimited string format for easy bulk editing. 

To add a new location, find the `const locationData` variable in the `<script>` tag and add a new line using the following format:

```text
Name | Country | Latitude | Longitude | Details
