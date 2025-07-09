# GTA V Color Mapping Project

A comprehensive analysis of vehicle color data, complete with processing scripts and visual assets. This project provides a clean dataset and tools to explore trends in vehicle colors.

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Data Sheets](https://img.shields.io/badge/Sheets-18-green.svg)](#data-overview)
[![Total Colors](https://img.shields.io/badge/Colors-8000+-red.svg)](#data-overview)
[![Community](https://img.shields.io/badge/Community-Driven-orange.svg)](#contributing)

[![GitHub stars](https://img.shields.io/github/stars/webshoppe/gta-color-mapping-project?style=social)](https://github.com/webshoppe/gta-color-mapping-project/stargazers) [![GitHub forks](https://img.shields.io/github/forks/webshoppe/gta-color-mapping-project?style=social)](https://github.com/webshoppe/gta-color-mapping-project/fork)

*"Because finding the perfect shade of Midnight Parasite Purple shouldn't require a computer science degree."*

---

## 🎯 What Makes This Special?

* **🎨 Comprehensive Coverage** – 8,000+ documented colors across 18 categories: Base colors, Custom hex codes, Crew colors, Vehicle liveries, Chameleon and Pearl paints, Headlights, Neon lights, Tire Smoke and more
* **👁️ Visual-First Design** – Every entry includes a 200×112px color swatch and a cell for a resized preview image (many with in-game preview images)
* **🤖 Mod-Ready Data** – Clean `.xlsx` masters, UTF-8 CSVs with flattened headers, and vehicle display name → model hash and color id mapping via DurtyFree's authoritative `vehicles.json` and `vehicleColors.json`
* **📋 Excel/LibreOffice Tooltips** – Hover any paint chip cell for instant spec sheet (Vehicle, Livery, Hex, Crew Code, Color Family)
* **🔗 Stable IDs** – Vehicle Model IDs link to spawn names, so your bookmarks and scripts won't break across updates
* **📚 Battle-Tested Sources** – Rebuilt from Wayback snapshots of joonasprkl's legendary archive, plus GTAForums, Se7enSins, GTA Wiki, Discord communities, and extensive field testing

*The definitive, community-driven reference for **every** paint-related value in Grand Theft Auto Online.*

---

### Note on Excel as the Primary Format for Color Accuracy

We chose Excel (`.xlsx`) as the primary format for this project because it provides the most accurate and vibrant color rendering for our swatches and paint chips. 

In our testing:
- Excel displays color fills and image swatches with the closest match to in-game colors.
- LibreOffice (`.ods`) files consistently show colors slightly darker or muted, even though the hex codes remain correct.
- Google Sheets typically displays colors somewhere between Excel and LibreOffice, but is optimized for Excel compatibility.

For the most reliable and visually accurate experience, especially when referencing specific shades or matching to in-game visuals, we recommend viewing the data in Excel. The `.ods` and `.csv` versions remain available for compatibility and data workflows, but may not represent colors exactly as intended.

---

## 🗂️ Data Overview

| Sheet Category | Rows | What's Inside | Unique Features |
|----------------|-----:|---------------|-----------------|
| **Base** | 223 | Official carcols palette with pearlescent pairings | Rank/win unlock requirements, texture types |
| **Custom** | 477 | Community hex colors with known crew codes | Verified crew codes, color family classification |
| **Crew** | 1,215 | Unnamed crew colors with known crew codes, awaiting color name identification | Crowd-sourced discovery project |
| **Livery** | 3,250 | **Rebuilt joonasprkl archive** – vehicle liveries matched to paint codes | Preview images, vehicle model mapping |
| **Chameleon** | 62 | Pearl/Flip/Prismatic/Holographic paints | GTA+ unlock status, effect types |
| **Pearlescent** | 75 | Pealecent colors applied to Metallic | Unlock conditions |
| **Neon Light** | 14 | Under-glow RGB values | Installation requirements |
| **Tire Smoke** | 15 | Smoke tint colors | Unlock conditions |
| +10 more | 1,500+ | Headlights, Wheels, Trim, Accent, Matte, Metallic, etc. | Category-specific unlock data |

> **💡 Pro Tip**: Columns like `Crew Code(s)` contain leading zeros (`00`) – import CSVs as **Text** type to preserve them!

---

## 🚀 Quick Start

### For General Users
1. **Download** → Grab `GTA_Color_Mapping_MASTER_v1.0.xlsx` and/or `GTA_Color_Mapping_MASTER_v1.0.ods` from [releases/](https://github.com/webshoppe/gta-color-mapping-project/releases)
2. **Open in Excel/LibreOffice** or **Upload and open in Google Sheets** → All formatting, images, and tooltips preserved
3. **Browse by category** → Use the TOC sheet for quick navigation
4. **Hover for details** → Paint chip cells show mini spec sheets

### For Modders & Developers

**Clone everything for local development**
`git clone https://github.com/webshoppe/gta-color-mapping-project.git`
`cd gta-color-mapping-project`

**Set up Python environment for data processing**
`python -m venv venv`
`source venv/bin/activate # Windows: venv\Scripts\activate`
`pip install -r scripts/requirements.txt`

---

## 🌟 Community Ecosystem

### Where This Data Lives
* **🎮 In-Game** → Modshops, Auto Shops, Agency, Arena, LSCM, etc.
* **🎨 Content Creation** → YouTube tutorials, Reddit showcases, Discord galleries, Community forums

### Related Projects & Inspiration

| Project | What It Offers | How We Differ |
|---------|----------------|---------------|
| **[joonasprkl/liverycolors Wayback Archive](https://web.archive.org/web/20201019023108/https://joonasprkl.github.io/liverycolors/)** | OG livery → color lookup (2016-2020) | ✅ **We rebuilt & expanded it** – fixed broken images, added model hashes, XLSX format |
| **[DurtyFree/gta-v-data-dumps](https://github.com/DurtyFree/gta-v-data-dumps)** | Raw game files (vehicles.json, vehicleColors, etc.) | ✅ **We consume their dumps** for authoritative model and color mapping |
| **[GTA Wiki - Respray Colors](https://gta.fandom.com/wiki/Vehicle_Customization_in_GTA_V/Respray_Colors)** | Full catalog of all things GTA with stats, customizations, vehicles, wheels, categories, missions, unlocks and more. | ✅ **Reformatted some color table data** for cross-referencing stats, customizations, vehicles, wheels, categories, unlocks, preview images and more. |
| **[GTABase - Vehicles](https://www.gtabase.com/grand-theft-auto-v/vehicles/)** | Comprehensive and uique GTA game databases | ✅ **Cross-referenced information** for vehicles, liveries, properties, aquisition methods, customizations, user builds, etc. |
| **Various pastebin/spreadsheet collections** | Custom colors, crew code lists, tats, cross referencing related stats, and more. | ✅ **Comprehensive, verified database** with provenance |

---

## 🎮 Community Servers & Resources

| Community | Focus | Link |
|-----------|-------|-------------|

| **GTAForums Color Section** | Historical discussions, rare finds | [GTAForums.com](https://gtaforums.com/) |
| **Se7enSins GTA Section** | Console modding, save editing | [Se7enSins.com](https://www.se7ensins.com/) |
| **GTA5-Mods.com** | GTA 5 car mods, scripts, tools and more | [GTA5-Mods.com](https://www.gta5-mods.com/) |
| **UnKnoWnCheaTs** | GTA 5 modding, stats, data, vehicle mods, etc | [UnKnoWnCheaTs.me/forum/grand-theft-auto-v](https://www.unknowncheats.me/forum/grand-theft-auto-v/) |

*Got a color-focused community? [Open a PR](CONTRIBUTING.md) to get listed!*

---

## 📊 Using The Data

### CSV Import (Preserves Leading Zeros)
**Excel**: Data → From Text/CSV → Set "Crew Code(s)" column to **Text** type  
**LibreOffice**: File → Open → Text Import → Set "Crew Code(s)" column type to **Text**  
**Google Sheets**: File → Import → Disable "Convert text to numbers"

---

## 🤝 Contributing

### 🆕 New Colors
1. **Fork this repo** and create a feature branch
2. **Add to appropriate sheet**: Base (official), Custom (community), or Crew (unknown names)
3. **Required fields**: Hex code, RGB values, 200×112px swatch PNG
4. **Bonus points**: In-game preview image, crew code verification, unlock conditions

### 🐛 Data Corrections
* **Wrong hex/RGB values**: Include screenshot evidence + source
* **Missing crew codes**: Test in-game or provide reliable source  
* **Broken images**: Replace with working URL or attach new image

### 🛠️ Code Improvements  
* **Script enhancements**: Tooltip generation, batch processing, validation
* **Documentation**: Usage guides, API examples, integration tutorials
* **Tooling**: Color conversion utilities, swatch generators

**See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines**

---

## 📈 Project Stats

* **Contributors**: 50+ community members
* **Data Sources**: Wayback Machine, Archive.today, github, 8 forums, 12 Discord servers, field testing
* **Last Major Update**: January 2025 (Vehicle ID mapping refresh)
* **Next Milestone**: Complete crew color identification project

---

## 📜 Legal & Attribution

### License
* **Code & Data**: MIT License – do whatever you want, just keep the copyright notice
* **Game Assets**: Screenshots/references © Rockstar Games, used under fair use for documentation
* **Community Contributions**: Credited in [CONTRIBUTORS.md](CONTRIBUTORS.md)

### Data Provenance
This project rebuilds and expands upon:
* **joonasprkl's legendary liverycolors archive** (2016-2020) – the foundation of GTA color mapping
* **Community contributions** from GTAForums, Se7enSins, Reddit, and Discord
* **DurtyFree's authoritative GTA data dumps** for color, vehicle and model hashing
* **Original research** by project maintainers and volunteer testers

---

## Made with ❤️ by the GTA Color Mapping Crew

*A worldwide community of modders, designers, and car enthusiasts who believe every pixel-perfect paint job deserves proper documentation.*

**[Download the data](data/) • [Report issues](issues/) • [Star the repo ⭐](../../stargazers)**

---
