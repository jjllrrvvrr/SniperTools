# Sniper Tools

Professional web-based calculators for precision shooting and sniper operations.

🔗 **Live Demo:** [https://jjllrrvvrr.github.io/SniperTools/](https://jjllrrvvrr.github.io/SniperTools/)

---

## Overview

Sniper Tools is a collection of specialized calculators designed for snipers, precision shooters, and tactical instructors. Built with a clean monochrome interface and responsive design, these tools work seamlessly across desktop and mobile devices, even offline.

All calculators feature:
- **Dark/Light mode** toggle with persistent preference
- **Responsive design** optimized for field use
- **Offline capability** - works without internet
- **No tracking or data collection** - everything stays local

---

## Tools

### 1. Loophole Calculator

Calculate bullet trajectory through obstacles to determine safe firing solutions.

**Purpose:** Determine if you can shoot through a small opening (loophole) without hitting the obstacle, based on your rifle's height-over-bore and dialed elevation.

**Features:**
- Rifle presets (AX338, SCAR-HPR, Barret .50)
- Visual sight picture with crosshair overlay
- GO/NO-GO decision indicator
- Aim point recommendation (top/bottom third)
- Real-time bullet path calculation

**Formula:** `Bullet Path = -(HOB × 10 / Distance) + Dialed Elevation`

---

### 2. Range Finder

Estimate target distance using mil-dot reticle measurements.

**Purpose:** Calculate distance to target based on its known size and angular measurement in mils.

**Features:**
- 8 preset target types (180cm standing man to 400cm vehicle)
- Custom size input
- Interactive slider (0.1 - 10 mils)
- Real-time distance calculation
- Formula display

**Formula:** `(Size in meters / Mils) × 1000 = Distance in meters`

---

### 3. MGRS Calculator

Calculate distance and bearing between two MGRS coordinates.

**Purpose:** Grid navigation and target location using Military Grid Reference System coordinates.

**Features:**
- Distance calculation (meters when <1km, kilometers when ≥1km)
- Bearing in degrees (0-360°) and mils (0-6400)
- Direction indicator with cardinal points (↑ ↗ → etc.)
- Calculation history (last 5)
- Smart grid reference handling: fill Zone/Square for one point, the other inherits it
- Cross-zone calculations supported
- Accurate MGRS-to-Lat/Lon conversion using proven algorithms

---

### 4. Unit Converter

Convert between metric and imperial units for distance and angular measurements.

**Purpose:** Quick conversion between different measurement systems commonly used in precision shooting.

**Features:**
- **Distance:** mm, cm, m, km, inches, feet, yards, miles
- **Angle:** degrees, mils, MOA, radians
- Bidirectional conversion (edit either field)
- Swap button for quick unit inversion
- Quick reference presets

**Examples:**
- 100m = 109.36 yards
- 1 MOA = 0.291 mils
- 1 mil = 3.438 MOA

---

### 5. Judging Distance Skills

Training tool for distance estimation exercises.

**Purpose:** Practice and validate distance estimation with configurable acceptance margins.

**Features:**
- 10 independent targets
- Configurable distance ranges with percentage margins
- Min/Max acceptable values calculated automatically
- Visual alert for distances >1000m
- Local storage for training session continuity

**Default Ranges:**
- 0-300m: ±15%
- 301-600m: ±10%
- 601-1000m: ±5%
- >1000m: Alert + 5%

---

### 6. Useful Links

Collection of reference links for precision shooters.

**Purpose:** Quick access to external resources, manuals, and references.

**Links include:**
- NATO Ballistic Data (AXMC, SCAR-H, M107A1)
- Precision shooting resources (6mm BR, Norma, Berger)
- Tactical guides and manuals
- Social media: @Belgiansniper Instagram

---

## Design

**Visual Identity:**
- Monochrome color scheme (no blue)
- Clean, minimalist interface
- High contrast for outdoor visibility
- Consistent header with logo navigation

**Technical:**
- Pure HTML/CSS/JavaScript - no frameworks
- CSS custom properties for theming
- LocalStorage for persistence
- Mobile-first responsive design

---

## Usage

### Desktop
1. Open `index.html` or visit the live demo
2. Select a tool from the grid
3. Click the logo to return home

### Mobile
- Add to home screen for quick access
- Works offline after first load
- Touch-optimized controls

---

## File Structure

```
SniperTools/
├── index.html              # Landing page
├── loophole.html           # Loophole Calculator
├── rangefinder.html        # Range Finder (mil-dot)
├── mgrscalculator.html     # MGRS Calculator
├── jd.html                 # Judging Distance Skills
├── styles.css              # Common stylesheet
├── logo.png                # Application logo
└── README.md               # This file
```

---

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile Safari & Chrome

---

## Data & Privacy

All data is stored locally in your browser:
- Theme preference (`sniperTheme`)
- Range Finder settings
- MGRS calculation history
- JD custom ranges and values

**No data is transmitted to any server.**

---

## Author

Created by [@jjllrrvvrr](https://github.com/jjllrrvvrr)

---

## License

Open source. Use, modify, distribute freely.
