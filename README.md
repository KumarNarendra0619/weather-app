<div align="center">

# 🌦️ Weather App

### A single-file, zero-dependency weather dashboard with live data, maps, and exports

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-View_App-3b82f6?style=for-the-badge)](https://kumarnarendra0619.github.io/weather-app/)
[![GitHub Pages](https://img.shields.io/github/deployments/KumarNarendra0619/weather-app/github-pages?style=for-the-badge&label=Pages&logo=github)](https://kumarnarendra0619.github.io/weather-app/)
[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](#-license)
[![Made with HTML](https://img.shields.io/badge/Made%20with-HTML%2FCSS%2FJS-e34f26?style=for-the-badge&logo=html5&logoColor=white)](#)

<img src="https://api.iconify.design/emojione-v1:sun-behind-cloud.svg" width="90" alt="weather icon" />

**No build step. No frameworks. No server. Just open `index.html`.**

</div>

---

## ✨ Features

<table>
<tr>
<td width="50%" valign="top">

### 🔎 Search & Location
- 🏙️ City search powered by Open‑Meteo geocoding
- 📍 "Use my location" via browser geolocation
- 🕘 Recent searches saved as quick-access chips
- 🎯 GPS accuracy + data-source accuracy scoring

</td>
<td width="50%" valign="top">

### 🌡️ Live Weather Data
- Current temperature, feels-like, humidity, dew point
- Wind speed/gusts/direction, pressure, visibility
- Cloud cover, UV index, precipitation, snowfall
- 5-day forecast with sunrise/sunset & rain probability

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🗺️ Multi-Provider Maps
- Google Maps · OpenStreetMap · Bhuvan · Aerial imagery
- Zoom in / zoom out controls
- DigiPIN lookup for precise Indian geo-addressing

</td>
<td width="50%" valign="top">

### 📤 Data Export
- ⚡ One-click fast export (daily + monthly + annual)
- 📅 Daily CSV — full current forecast breakdown
- 📆 Monthly / 📈 Annual aggregated CSV via historical archive
- 🌓 °C / °F toggle, persisted across sessions

</td>
</tr>
</table>

---

## 🚀 Quick Start

```bash
# Clone it
git clone https://github.com/KumarNarendra0619/weather-app.git
cd weather-app

# Open it — that's it, no install step
start index.html      # Windows
open index.html        # macOS
xdg-open index.html    # Linux
```

Or just visit the **[live demo](https://kumarnarendra0619.github.io/weather-app/)** — hosted free on GitHub Pages. 🎉

---

## 🧭 How It Works

```mermaid
flowchart LR
    A[🔎 City Search / 📍 Geolocation] --> B[Open-Meteo Geocoding API]
    B --> C[Open-Meteo Forecast API]
    C --> D[🎨 Render current + 5-day cards]
    D --> E[🗺️ Update map provider]
    C -.fetch fails.-> F[💾 Cached data]
    F -.no cache.-> G[📦 Hardcoded fallback data]
    D --> H[📤 CSV Export: daily / monthly / annual]
```

---

## 🎨 Design Highlights

| Aspect | Details |
|---|---|
| 🖋️ Typography | Sans-serif, 15px body, system font stack |
| 🌗 Theming | Auto light/dark via `prefers-color-scheme` |
| 🎨 Accent color | Dynamically shifts per weather condition |
| 📱 Layout | Centered narrow column, fully responsive |
| ♿ Accessibility | `prefers-reduced-motion` respected, ARIA labels on controls |

---

## 🗂️ Tech Stack

<div align="left">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Open-Meteo](https://img.shields.io/badge/API-Open--Meteo-0ea5e9?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-181717?style=flat-square&logo=github&logoColor=white)

</div>

No npm, no bundlers, no backend — a single portable `index.html` file.

---

## 📁 Repository Structure

```
weather-app/
└── index.html   # 🎯 Everything: markup, styles, and logic in one file
```

---

## 🤝 Contributing

Pull requests are welcome! Ideas for future enhancements:

- [ ] Hourly forecast view
- [ ] Weather alerts / severe warnings
- [ ] PWA offline support
- [ ] Additional language localization

---

## 📄 License

Released under the **MIT License** — free to use, modify, and share.

<div align="center">

Made with ☀️ 🌧️ ❄️ and Copilot

</div>
