# Sniper Tools

A collection of professional web-based calculators for sniper training and precision shooting.

## 🎯 Overview

Sniper Tools provides specialized calculators designed for:
- **Sniper training exercises** - Distance estimation practice
- **Precision shooting** - Quick calculations in the field
- **Instructor tools** - Configurable parameters for training scenarios

## 🛠️ Tools Included

### 1. Judging Distance Calculator (`jd.html`)
A training aid for distance estimation exercises.

**How it works:**
- Instructor enters the actual target distance
- The calculator displays the acceptable Min/Max range based on configurable percentage margins
- Trainee's estimate is valid if it falls within this range

**Features:**
- **10 configurable targets** - Manage multiple training scenarios
- **Real-time calculation** - Instant Min/Max range display
- **Customizable ranges** - Configure your own distance thresholds and percentages
- **Visual alerts** - Warning for distances >1000m

### 2. Mil-Dot Master (`mildotmaster.html`)
An interactive slide rule for calculating distances using mil-dot reticle measurements.

**How it works:**
- Select target type (standing man, crouched, head/shoulders, etc.)
- Enter mils observed through scope
- Get instant distance calculation
- Or use the interactive slide rule by dragging

**Features:**
- **8 reference targets** - From helmet (25cm) to vehicle (400cm)
- **Interactive slide rule** - Drag to align values
- **Dual input** - Slider or numeric entry
- **Real-time calculation** - Formula displayed: `(Size × 10) ÷ Mils = Distance`

## ✨ Common Features

### Design
- **Clean monochrome design** - Black, white, and gray color scheme
- **Large logo** - Prominent branding (120px on desktop)
- **Responsive layout** - Works on desktop, tablet, and mobile
- **Consistent navigation** - Click logo to return to home

### Theme Support
- **Dark/Light mode** - Toggle with animated sun/moon icons
- **Synchronized** - Theme preference shared across all tools via LocalStorage
- **Persistent** - Your preference is saved automatically

### Technical
- **No dependencies** - Vanilla HTML, CSS, JavaScript
- **Offline capable** - Works without internet after first load
- **Local storage** - Saves your data and preferences
- **Common stylesheet** - Consistent styling across tools (`styles.css`)

## 🚀 Usage

### Getting Started
1. Open `index.html` to view available tools
2. Click on a tool card to launch it
3. Click the Sniper Tools logo to return home

### Judging Distance Calculator
1. Configure distance ranges via the ⚙️ gear icon (optional)
2. Enter actual distances for each target
3. Read the Min/Max columns for acceptable estimation ranges

### Mil-Dot Master
1. Select target type from dropdown
2. Enter mils observed (use slider or type value)
3. Read calculated distance
4. Or drag the slide rule to visually align values

## 🛠️ Technical Details

### Technologies
- **HTML5** - Semantic markup
- **CSS3** - Custom properties (CSS variables), Grid, Flexbox
- **JavaScript** - Vanilla JS, no frameworks
- **LocalStorage API** - Data persistence across sessions

### File Structure
```
SniperTools/
├── index.html              # Landing page with tool selection
├── jd.html                 # Judging Distance Calculator
├── mildotmaster.html       # Mil-Dot Master
├── styles.css              # Common stylesheet
├── logo.png                # Application logo
└── README.md               # This file
```

### Browser Compatibility
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 💾 Data Storage

The application uses browser LocalStorage to save:
- **Theme preference** - Light or dark mode (shared across tools)
- **JD Calculator** - Custom ranges and target values
- **Mil-Dot Master** - Last used settings

**Note:** All data is stored locally in your browser. Nothing is transmitted to any server.

## 🔒 Privacy

This application:
- ✅ Stores data only in your browser's LocalStorage
- ✅ Works completely offline
- ✅ Does not transmit any data to servers
- ✅ Does not use cookies or tracking

## 🎨 Customization

### Modifying Default Values
Edit the source files to customize:
- Distance ranges in `jd.html`
- Target sizes in `mildotmaster.html`
- Colors in `styles.css`

## 📝 License

This project is open source. Feel free to use, modify, and distribute.

## 👤 Author

Created by [jjllrrvvrr](https://github.com/jjllrrvvrr)

## 🤝 Contributing

Suggestions and improvements are welcome! Feel free to:
- Fork the repository
- Submit pull requests
- Report issues
- Suggest new features or tools

---

**Live Demo:** https://jjllrrvvrr.github.io/SniperTools/