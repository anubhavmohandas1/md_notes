# 🎵 Musicians' Den - Note Spinner

A visually stunning, interactive musical note practice tool designed for **Musicians' Den**, Ahmedabad.

**Live Demo:** Upload `note_spinner_final_v2.html` to your server and open in browser.

---

## Features

### 🎡 Spinning Wheel
- 12 musical notes: C, C#/D♭, D, D#/E♭, E, F, F#/G♭, G, G#/A♭, A, A#/B♭, and B
- Rainbow gradient colors for each note
- Smooth 4-second spin animation with easing
- Counter-rotating labels (always readable)
- Glowing gold border with pulse animation

### 🎮 Controls
| Button | Function |
|--------|----------|
| ▶ Play | Spin the wheel |
| ‖ Pause | Pause auto-roll countdown |
| ■ Stop | Stop and reset |

### ⚙️ Settings

| Setting | Description | Default |
|---------|-------------|---------|
| Auto Roll | Automatically spin again after delay | ON |
| Delay | Seconds between auto spins (1-60) | 5 sec |
| Audio 🔊 | Enable/disable sound effects | OFF |

### 🎨 Visual Effects
- Floating music notes background (♪ ♫ ♬)
- Confetti explosion on win
- Sparkle effects around result
- Pulsing center circle
- Highlighted winning segment
- Gradient buttons with hover effects

### 🔊 Audio (Optional)
- **Tick sounds:** Soft chimes while spinning
- **Win sound:** Gentle arpeggio in the selected note's frequency
- Musical and soothing - appropriate for instrument practice

---


## Usage Guide

### For Students
1. Open the Note Spinner page
2. Click **Play** to spin
3. Practice the note shown on your instrument
4. With **Auto Roll ON**, it will automatically show new notes

### For Teachers
- Set **Delay** to give students time to find/play the note
- Use in class for random note recognition exercises
- Works on mobile devices for individual practice

---

## Customization

### Change Colors
Edit `noteColors` array in JavaScript:
```javascript
const noteColors = [
    ['#ff6b6b', '#ee5a5a'], // C - gradient start, end
    // ... more colors
];
```

### Change Spin Duration
Edit wheel CSS transition:
```css
.wheel {
    transition: transform 4s cubic-bezier(...); /* Change 4s */
}
```
Also update `duration` variable in `spin()` function.

### Change Notes
Edit `notes` array:
```javascript
const notes = ['C', 'C#', 'Db', ...];
```

### Add/Remove Effects
- Confetti: Remove `createConfetti()` call in `showResult()`
- Sparkles: Remove `createSparkles()` call
- Floating notes: Remove `createFloatingNotes()` call

---

## Browser Support

| Browser | Support |
|---------|---------|
| Chrome | ✅ Full |
| Firefox | ✅ Full |
| Safari | ✅ Full |
| Edge | ✅ Full |
| Mobile Browsers | ✅ Full |

**Note:** Audio requires user interaction first (browser policy). Click Play to enable.

---


---

## Technical Details

- **Pure HTML/CSS/JS** - No frameworks or libraries required
- **Single file** - Everything contained in one HTML file
- **CDN dependency** - Google Fonts (Poppins) only
- **Web Audio API** - For sound generation
- **SVG** - For wheel segments
- **CSS Animations** - For all visual effects
- **Responsive** - Works on all screen sizes

---

## Credits

**Developed for:** Musicians' Den, Ahmedabad  
**Website:** [musiciansdenindia.com](https://musiciansdenindia.com)  
**Contact:** +91 84016 40325  
**Email:** musiciansden112@gmail.com

---

## License

© 2026 Musicians' Den. All rights reserved.

For use by Musicians' Den only. Do not redistribute without permission.
