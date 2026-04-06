# JD Calculator - Sniper Judging Distance Calculator

A web-based calculator for sniper training exercises, designed to help instructors evaluate distance estimation skills.

## 🎯 Purpose

In sniper training, targets are placed at various distances. Trainees must estimate these distances by eye. This calculator determines the acceptable estimation range (Min/Max values) based on the actual distance, using configurable percentage margins.

**How it works:**
- Instructor enters the actual target distance
- The calculator displays the acceptable Min/Max range
- Trainee's estimate is valid if it falls within this range

## ✨ Features

### Core Functionality
- **10 configurable targets** - Manage multiple training scenarios
- **Real-time calculation** - Instant Min/Max range display
- **Dark/Light mode** - Toggle between themes with animated sun/moon icons
- **Local storage** - Saves your data between sessions
- **Responsive design** - Works on desktop, tablet, and mobile

### Customizable Calculation Ranges
- **Configure distance ranges** - Click the ⚙️ gear icon in the "Calculation rules" section
- **Dynamic ranges** - Add or remove ranges (2-10 ranges supported)
- **Automatic continuity** - Ranges automatically adjust to prevent gaps or overlaps
- **Default values:**
  - 0-300m: ±15%
  - 301-600m: ±10%
  - 601-1000m: ±5%
  - >1000m: Alert + 5%

### User Interface
- **Clean monochrome design** - Black, white, and gray color scheme
- **Tabular layout** - Clear Target/Distance/Min/Max presentation
- **Visual alerts** - Orange border warning for distances >1000m
- **Centered inputs** - Easy-to-read distance entry
- **GitHub integration** - Link to creator's profile

## 🚀 Usage

### Basic Usage
1. Open `index.html` in any modern web browser
2. Enter the actual distance for each target in meters
3. The Min and Max columns automatically display the acceptable estimation range
4. Trainees should estimate within this range to pass

### Customizing Ranges
1. Click the ⚙️ gear icon next to "Calculation rules"
2. Modify distance thresholds and percentage values
3. Click "Add range" to create additional ranges (up to 10)
4. Click "Reset to default values" to restore original settings

### Theme Toggle
- Click the sun/moon toggle in the header to switch between light and dark modes
- Your preference is saved automatically

## 🛠️ Technical Details

### Technologies
- **HTML5** - Semantic markup
- **CSS3** - Custom properties (variables), Grid, Flexbox, transitions
- **JavaScript** - Vanilla JS, no dependencies
- **LocalStorage API** - Data persistence

### Browser Compatibility
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

### File Structure
```
JD/
├── index.html          # Main application
├── logo.png            # Application logo
└── README.md           # This file
```

## 💾 Data Storage

The application uses browser LocalStorage to save:
- **Target distances** - All 10 target values
- **Theme preference** - Light or dark mode
- **Custom ranges** - Your configured calculation ranges

**Note:** Data is stored locally in your browser and is not transmitted to any server.

## 🎨 Customization

### Changing Default Ranges
Edit the `defaultRanges` array in the JavaScript section:

```javascript
const defaultRanges = [
  { min: 0, max: 300, percent: 15 },
  { min: 301, max: 600, percent: 10 },
  { min: 601, max: 1000, percent: 5 },
  { min: 1001, max: null, percent: 5 }  // null = Infinity
];
```

### Color Scheme
The monochrome theme uses CSS custom properties. Edit the `:root` section to adjust colors.

## 📱 Mobile Support

The calculator is fully responsive:
- **Desktop:** Full table view with all columns
- **Tablet:** Optimized spacing
- **Mobile:** Stacked layout with labeled Min/Max cells

## 🔒 Privacy

This application:
- ✅ Stores data only in your browser's LocalStorage
- ✅ Works completely offline
- ✅ Does not transmit any data to servers
- ✅ Does not use cookies or tracking

## 📝 License

This project is open source. Feel free to use, modify, and distribute.

## 👤 Author

Created by [jjllrrvvrr](https://github.com/jjllrrvvrr)

## 🤝 Contributing

Suggestions and improvements are welcome! Feel free to:
- Fork the repository
- Submit pull requests
- Report issues
- Suggest new features

---

**Live Demo:** https://jjllrrvvrr.github.io/SniperTools/
