# 🎮 Brylas Super Bros - Interactive HTML5 Platformer

**A high-performance, responsive platformer game showcasing JavaScript state management and collision detection**

---

## 🎯 Overview

**Brylas Super Bros** is a fully-featured mobile-responsive platformer game built with vanilla JavaScript and HTML5 Canvas. This project demonstrates:

- ✨ **Custom collision detection** engine
- ✨ **Frame-based animation system** with sprite management
- ✨ **Mobile-first responsive design**
- ✨ **Advanced state management** in JavaScript (ES6+)
- ✨ **Performance optimization** for smooth 60 FPS gameplay

Designed as a portfolio piece showcasing the ability to engineer complex, interactive systems from the ground up.

---

## 🚀 Features

### 🎮 **Core Gameplay**
- Responsive platformer mechanics
- Gravity and physics simulation
- Enemy AI and collision response
- Power-ups and collectibles
- Level progression system

### 📱 **Cross-Platform Support**
- Desktop (keyboard controls)
- Mobile/Tablet (touch controls)
- Fully responsive UI
- Touch event handling optimization

### 🎨 **Visual Design**
- Sprite-based graphics with animation
- Real-time collision visualization (debug mode)
- Smooth camera following
- Dynamic level backgrounds

### 🔊 **Audio**
- Background music
- Sound effects for actions (jump, collect, hit)
- Volume controls
- Audio context management

### ⌨️ **Input Systems**
- **Keyboard**: Arrow keys / WASD for movement, Space to jump
- **Touch**: Swipe left/right, tap to jump
- **Mobile**: Optimized touch zones

---

## 🎮 How to Play

### Quick Start
1. **Open** `index.html` in a modern web browser
2. **Use keyboard** or touch controls
3. **Collect coins** and reach the goal 🎯

### Controls

| Input | Action |
|-------|--------|
| **← / →** (Arrow Keys) | Move left/right |
| **W / A / D** | Move (alternative) |
| **SPACE** | Jump |
| **Touch (Mobile)** | Swipe left/right to move |
| **Tap (Mobile)** | Tap screen to jump |
| **P** | Pause/Resume |
| **R** | Restart level |
| **M** | Mute/Unmute audio |

---

## 🛠️ Technical Architecture

### State Management
```javascript
// Global game state using ES6+ patterns
const gameState = {
  player: { x, y, velocity, direction },
  level: { current, completed, score },
  entities: [ /* enemies, collectibles, platforms */ ],
  camera: { x, y },
  audio: { muted, volume }
}
```

### Collision Detection
- **AABB (Axis-Aligned Bounding Box)** for efficient collision checks
- **Spatial partitioning** to optimize collision queries
- **Response handling** for different collision types
- Real-time debug visualization available

### Game Loop
- **60 FPS target** with delta-time calculations
- **requestAnimationFrame** for smooth animation
- **Optimized rendering** with dirty rectangle updates
- **Mobile-friendly** frame rate adaptation

### Mobile Optimization
- **Touch event debouncing** to prevent duplicate actions
- **Viewport scaling** for proper canvas rendering
- **Gesture detection** for swipe controls
- **Battery-conscious** frame rate on mobile

---

## 📊 Project Stats

| Metric | Value |
|--------|-------|
| **Language** | JavaScript (ES6+) |
| **Lines of Code** | ~2000+ |
| **File Size** | ~85 KB |
| **Load Time** | <1 second |
| **Target FPS** | 60 |
| **Mobile Support** | Full |

---

## 🔧 Troubleshooting

| Problem | Solution |
|---------|----------|
| Game doesn't respond to keyboard | Click canvas to focus, then try keys |
| Touch controls not working | Ensure browser supports Touch Events |
| Sprites not loading | Check image paths in code |
| Performance is choppy | Try reducing resolution or closing other browser tabs |
| Audio not playing | Check browser audio permissions |

---

## 💻 System Requirements

- **Browser**: Chrome, Edge, Firefox, Safari (modern versions)
- **OS**: Windows, macOS, Linux, iOS, Android
- **Internet**: Not required (offline-capable)
- **Resolution**: 800x600 minimum recommended

---

## 🛠️ Development & Customization

### File Structure
```
Brylas_super_boss/
├── index.html          # Main game file (HTML + CSS + JS)
├── README.md           # This file
├── assets/             # Game sprites and sounds
│   ├── sprites/
│   └── audio/
└── .gitignore
```

### Quick Customization

**Change player sprite:**
```javascript
// In the JS section, find:
player.sprite = new Image();
player.sprite.src = 'assets/sprites/player.png';
```

**Adjust difficulty:**
```javascript
// Modify these constants:
GRAVITY = 0.6;           // Lower = lighter jumps
JUMP_POWER = 15;         // Higher = higher jumps
ENEMY_SPEED = 2;         // Higher = faster enemies
```

**Add new levels:**
```javascript
// Add to the levels array
const levels = [
  { width: 1600, height: 600, ... },
  { width: 2000, height: 700, ... }, // New level
];
```

---

## 🎓 Learning Outcomes

This project demonstrates mastery of:

✅ **State Management** - Complex game state handling in vanilla JS  
✅ **Collision Detection** - Custom physics engine  
✅ **Animation Systems** - Sprite-based animation with timing  
✅ **Event Handling** - Keyboard and touch input processing  
✅ **Performance Optimization** - Achieving 60 FPS on constrained devices  
✅ **Responsive Design** - Mobile-first approach  
✅ **Canvas API** - Low-level graphics rendering  
✅ **Audio API** - Sound management and playback  

---

## 📈 Roadmap

Future enhancements:
- 🎨 Power-up system (speed boost, shield, etc.)
- 🎵 Dynamic audio system with multiple tracks
- 🏆 Leaderboard with local storage
- 🌐 Multiplayer support (WebSockets)
- 📊 Analytics & telemetry
- 🎬 Recording & replay system

---

## 📄 License

This project is licensed under the **MIT License**.

Free to use, modify, and distribute - see [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**BrylasBit** - Interactive Web Games & Canvas Experiments

**Key Skills Demonstrated:**
- Advanced JavaScript (ES6+)
- HTML5 Canvas & WebGL
- State management patterns
- Mobile responsiveness
- Real-time performance optimization

---

## 🤝 Contributing

Contributions welcome! Feel free to:
- 🐛 Report bugs
- 💡 Suggest features
- 🔧 Submit pull requests
- 📸 Share improvements

---

## 📞 Support

Questions? Check the code comments or create a GitHub issue.

---

**Enjoy the game! 🎮**
