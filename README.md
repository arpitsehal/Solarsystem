# 🌌 3D Solar System - Three.js

An interactive 3D solar system built with vanilla JavaScript and Three.js, featuring all 8 planets with realistic orbital mechanics, customizable speed controls, and immersive camera navigation.

![Solar System Preview](https://img.shields.io/badge/Three.js-r128-blue) ![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow) ![Mobile](https://img.shields.io/badge/Mobile-Responsive-green)

## ✨ Features

- **🌟 Complete Solar System**: All 8 planets with realistic relative sizes and distances
- **🎮 Interactive Controls**: Individual speed sliders for each planet
- **🖱️ Camera Navigation**: Mouse/touch controls for orbiting and zooming
- **💡 Realistic Lighting**: Point light source from the sun with proper shadows
- **🌠 Visual Effects**: Glowing sun, star field background, planet tooltips
- **📱 Mobile Responsive**: Touch-friendly interface that works on all devices
- **🎨 Theme Toggle**: Dark/Light theme switching
- **⏯️ Animation Controls**: Pause/Resume and Reset functionality

## 🚀 Quick Start

### Option 1: Direct File Access (Simplest)

1. **Download the project**:
   ```bash
   # Clone or download the repository
   git clone https://github.com/yourusername/3d-solar-system.git
   cd 3d-solar-system
   ```

2. **Open in browser**:
   - Double-click `index.html`
   - Or right-click → "Open with" → Your browser

3. **That's it!** The solar system should load immediately.

### Option 2: Local Development Server (Recommended)

For development or if you encounter CORS issues:

#### Using Python:
```bash
# Navigate to project directory
cd 3d-solar-system

# Python 3.x
python -m http.server 8000

# Python 2.x
python -m SimpleHTTPServer 8000

# Open: http://localhost:8000
```

#### Using Node.js:
```bash
# Install http-server globally
npm install -g http-server

# Run in project directory
cd 3d-solar-system
http-server -p 8000

# Open: http://localhost:8000
```

#### Using PHP:
```bash
# Navigate to project directory
cd 3d-solar-system

# Start PHP server
php -S localhost:8000

# Open: http://localhost:8000
```

### Option 3: VS Code Live Server

1. Install the "Live Server" extension in VS Code
2. Open `index.html` in VS Code
3. Right-click → "Open with Live Server"
4. Browser opens automatically

### Option 4: Online Editors (No Installation)

Copy and paste the code into any of these platforms:
- **CodePen**: https://codepen.io/pen/
- **JSFiddle**: https://jsfiddle.net/
- **Replit**: https://replit.com/
- **CodeSandbox**: https://codesandbox.io/

## 📁 Project Structure

```
3d-solar-system/
├── index.html              # Main HTML file with embedded CSS/JS
├── README.md              # This file
├── screenshots/           # Demo images (optional)
│   ├── solar-system.png
│   └── controls.png
└── docs/                  # Additional documentation (optional)
    ├── FEATURES.md
    └── DEVELOPMENT.md
```

## 🎯 Usage Guide

### Basic Navigation
- **Mouse Drag**: Orbit around the solar system
- **Mouse Wheel**: Zoom in/out
- **Touch Drag**: Mobile navigation
- **Pinch**: Mobile zoom

### Control Panel
- **Planet Speed Sliders**: Adjust orbital speed for each planet individually
- **Number Inputs**: Precise speed control (0-10 range)
- **Pause/Resume**: Stop/start all animations
- **Reset**: Return all planets to starting positions
- **Theme Toggle**: Switch between dark and light themes

### Interactive Features
- **Hover Tooltips**: Move mouse over planets to see information
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Real-time Updates**: All changes apply immediately

## 🔧 Requirements

### System Requirements
- **Internet Connection**: Required for Three.js CDN
- **Modern Browser**: Chrome 58+, Firefox 55+, Safari 12+, Edge 79+
- **JavaScript Enabled**: Must be enabled in browser settings

### Performance Requirements
- **RAM**: 1GB minimum (2GB recommended)
- **Graphics**: Hardware acceleration recommended
- **Screen**: Works on any screen size (320px minimum width)

## 🐛 Troubleshooting

### Common Issues

#### 1. Black Screen / Not Loading
```
Problem: Page loads but shows only black screen
Solution: 
- Check browser console (F12) for errors
- Verify internet connection (Three.js loads from CDN)
- Try using a local server (Option 2 above)
```

#### 2. Three.js Failed to Load
```
Problem: "THREE is not defined" error
Solution: 
- Check internet connection
- Try alternative CDN in index.html:
  <script src="https://unpkg.com/three@0.128.0/build/three.min.js"></script>
```

#### 3. Controls Not Working
```
Problem: Mouse/touch controls don't respond
Solution:
- Ensure you're clicking/dragging on the 3D scene area
- Refresh the page
- Check if JavaScript is enabled
```

#### 4. Poor Performance
```
Problem: Laggy animation or low frame rate
Solution:
- Close other browser tabs
- Reduce browser zoom level
- Try on a different device
- Check hardware acceleration is enabled
```

#### 5. Mobile Issues
```
Problem: Controls don't work on mobile
Solution:
- Try touch and drag instead of mouse
- Ensure browser supports WebGL
- Try landscape orientation
```

### Browser Compatibility

| Browser | Version | Status |
|---------|---------|---------|
| Chrome | 58+ | ✅ Fully Supported |
| Firefox | 55+ | ✅ Fully Supported |
| Safari | 12+ | ✅ Fully Supported |
| Edge | 79+ | ✅ Fully Supported |
| Opera | 45+ | ✅ Fully Supported |
| Mobile Chrome | 70+ | ✅ Fully Supported |
| Mobile Safari | 12+ | ✅ Fully Supported |

## 🔨 Development

### Making Changes

1. **Edit the HTML file** with any text editor
2. **Refresh browser** to see changes
3. **Use browser dev tools** (F12) for debugging

### Code Structure

- **HTML**: Basic structure and styling
- **CSS**: Responsive design and themes
- **JavaScript**: Three.js scene setup and animation logic

### Key Components

```javascript
// Main class structure
class SolarSystem {
    constructor()     // Initialize system
    setupScene()      // Create Three.js scene
    createPlanets()   // Generate planet objects
    setupControls()   // Build UI controls
    animate()         // Animation loop
}
```

### Adding New Features

1. **New Planet**: Add to `planetData` array
2. **New Controls**: Extend `setupControls()` method
3. **Visual Effects**: Modify materials and lighting
4. **UI Elements**: Add to HTML structure

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🆘 Support

If you encounter issues:

1. **Check this README** for common solutions
2. **Browser Console**: Check for JavaScript errors (F12)
3. **Try Different Browser**: Test in Chrome/Firefox
4. **Check Internet**: Verify Three.js CDN access
5. **Create Issue**: Report bugs with browser/system details

## 📊 Performance Tips

- **Close unused tabs** for better performance
- **Use hardware acceleration** in browser settings
- **Latest browser version** for best compatibility
- **Stable internet connection** for CDN resources

---

**Built by using Three.js and vanilla JavaScript**

*No frameworks, no build tools, just pure web technologies!*
