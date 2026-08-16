# 🎮 METAVERSE - Virtual Gaming Hub

A fully-featured 3D multiplayer gaming platform built with Three.js, featuring R6 blocky avatars, mini-games, customization, and social features.

## 🌟 Features

### 🎭 Avatar Customization
- **9 Starter Characters**: Cyber Knight, Astro Explorer, Dragon Master, Mystic Wizard, Shadow Ninja, Cyber Samurai, Phoenix Warrior, Frost Mage, Classic Guest
- **31+ Items**: 8 hats, 6 accessories, 9 skins, 8 pets, shoulder pals
- **R6 Blocky Style**: Classic Roblox-inspired character design
- **Real-time 3D Preview**: See your avatar in the game world

### 🎮 Mini-Games
1. **Coin Collector VR** - Catch falling coins with combo system
2. **Asteroid Survival** - Dodge meteors with health tracking
3. **Meta Parkour Rush** - Platform jumping with checkpoints
4. **Cyber Speed Race** - High-speed racing with obstacles
5. **Tower Climb Challenge** - Vertical platforming challenge
6. **Arena Battle Royale** - Survive waves of enemies

### 💬 Social Features
- **3-Tab Chat System**: Global, Game, and Friends chat
- **Friends System**: Add friends, see online status
- **Activity Feed**: Track your achievements and progress
- **Real-time Player Counts**: See how many players are in each game

### 🏆 Progression System
- **M$ Meta Coins**: Earn through gameplay, spend on items
- **Meta XP**: Level up by playing games
- **8 Achievements**: Unlock badges for milestones
- **Daily Rewards**: Claim M$ 200 + ⭐ 500 XP every 24 hours

### 📱 Modern Features
- **PWA Support**: Install as app on mobile/desktop
- **Offline Mode**: Service worker caching
- **Responsive Design**: Works on all devices
- **Auto-Input Detection**: Hides mobile controls on keyboard use
- **Account Switching**: Multiple accounts with quick switch
- **Guest Mode**: Play without creating account

### 🎯 Gameplay Mechanics
- **WASD Movement**: Full 3D world navigation
- **Space Bar Jumping**: Physics-based jumping with gravity
- **Platform Collision**: Proper collision detection
- **Camera Zoom**: Scroll wheel to zoom (3-25 units)
- **Portal Zones**: Walk into portals to open UI

## 📁 File Structure

```
game/
├── index.html           # Homepage with game carousel
├── website777.html      # Login/signup page
├── web777game.html      # Main game (150KB - all features)
├── manifest.json        # PWA manifest
├── service-worker.js    # Offline caching
├── DEPLOYMENT_GUIDE.md  # How to publish
└── README.md           # This file
```

## 🚀 Quick Start

### Local Testing
1. Open `index.html` in a web browser
2. Click "Login" or "Play as Guest"
3. Start playing!

### Deploy to Web
See [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md) for detailed instructions.

**Quick Deploy Options:**
- **Netlify**: Drag & drop folder → instant deploy
- **GitHub Pages**: Push to repo → enable Pages
- **Vercel**: Connect GitHub → auto-deploy

## 🎮 How to Play

### Controls
- **WASD / Arrow Keys**: Move character
- **Space Bar**: Jump
- **Mouse Scroll**: Zoom camera in/out
- **E Key**: Interact with portal zones
- **Enter**: Send chat message

### Getting Started
1. **Create Account**: Choose your starter avatar
2. **Explore Hub**: Walk around the 3D world
3. **Enter Portals**: 
   - 🛍️ SHOP Portal (left) - Buy items
   - 🎮 GAMES Portal (center) - Play mini-games
   - 👗 CLOSET Portal (right) - Customize avatar
4. **Earn Coins**: Play games to earn M$ and XP
5. **Customize**: Buy hats, pets, skins, and more!

## 💾 Technical Details

### Technologies
- **Three.js r128**: 3D rendering engine
- **Vanilla JavaScript**: No frameworks
- **LocalStorage**: Data persistence
- **Service Worker**: PWA offline support
- **CSS Grid/Flexbox**: Responsive layouts

### Browser Compatibility
- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Mobile browsers (iOS Safari, Chrome Android)

### Performance
- **Optimized**: ~150KB main game file
- **CDN Assets**: Three.js loaded from jsdelivr
- **Caching**: Service Worker caches all resources
- **No Images**: All icons use emojis (lightweight)

## 🔧 Customization

### Add New Items
Edit `CATALOG` array in `web777game.html`:
```javascript
{ 
  id: 'item_id', 
  name: 'Item Name', 
  category: 'hat', // or 'acc', 'skin', 'pet', 'pal'
  price: 500, 
  icon: '🎩', 
  color: 0x00A2FF 
}
```

### Add New Games
1. Create spawn function (e.g., `spawnMyGame()`)
2. Add game logic to `updateMiniGameLoop()`
3. Add game card to UI
4. Add to `startMiniGame()` switch statement

## 🐛 Known Issues & Fixes

### Issue: Can't jump in games
**Fixed!** Space bar jumping now works everywhere.

### Issue: Falling through platforms
**Fixed!** Platform collision detection implemented.

### Issue: Mobile controls always visible
**Fixed!** Auto-detects input device and hides controls on keyboard use.

### Issue: Chat messages not sending
**Fixed!** Added send button and improved Enter key handling.

## 🎨 Customization Options

### Change Theme Colors
Primary color: `#00A2FF` (cyan blue)
- Used in gradients, buttons, highlights
- Search and replace hex code to change theme

### Modify Currency Names
- M$ Meta Coins → Your currency name
- Meta XP → Your XP name
- Search and replace in all HTML files

### Add Custom Avatars
Edit `avatarStarterMap` in `website777.html`

## 📊 Version History

### v1.5.0 (Current)
- ✅ Jumping mechanics with gravity
- ✅ Platform collision detection
- ✅ Auto input device detection
- ✅ Shoulder pal companions
- ✅ Enhanced chat with send button
- ✅ Complete METAVERSE rebrand

### v1.0.0
- Initial release with 6 games
- Avatar customization
- Chat and friends system
- PWA support

## 📄 License

This project is open source. Feel free to use, modify, and distribute.

## 🤝 Contributing

Want to improve METAVERSE? 
1. Fork the project
2. Make your changes
3. Test thoroughly
4. Submit improvements

## 📞 Support

Having issues? Check:
1. Browser console for errors
2. LocalStorage is enabled
3. JavaScript is enabled
4. Using modern browser (2020+)

## 🎯 Future Roadmap

Potential features:
- [ ] Real multiplayer (Socket.io/Firebase)
- [ ] More mini-games
- [ ] Trading system
- [ ] Leaderboards
- [ ] Custom avatar creator
- [ ] Voice chat
- [ ] In-game currency purchases

## 🌐 Live Demo

After deployment, add your URL here:
- **Live Site**: `https://your-site.com`
- **GitHub**: `https://github.com/yourusername/metaverse-game`

---

**Made with ❤️ using Three.js**

*Ready to publish? See [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md)!*
