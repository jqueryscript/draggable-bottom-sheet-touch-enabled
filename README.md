# Draggable Bottom Sheet (Touch-Enabled)

A modern, touch-enabled draggable bottom sheet modal component built with vanilla HTML, CSS, and JavaScript. This component provides a smooth, interactive bottom sheet experience similar to popular mobile applications like Facebook and Instagram.

## ✨ Features

- 🎯 **Touch-Enabled**: Fully functional on both desktop and mobile devices
- 📱 **Responsive**: Adapts seamlessly to different screen sizes
- 🖱️ **Drag & Drop**: Intuitive drag gestures for sheet manipulation
- 🎨 **Smooth Animations**: CSS-powered transitions for fluid user experience
- 🔒 **Body Scroll Lock**: Prevents background scrolling when sheet is open
- 📐 **Height Snap Points**: Automatically snaps to 25%, 50%, or 100% viewport heights
- 🎪 **Fullscreen Mode**: Smoothly transitions to fullscreen when dragged high enough
- 💻 **Vanilla JavaScript**: No dependencies required - pure JS implementation

## 🚀 Demo

Try the live demo here: [https://codepen.io/iqq800/pen/QwNWrzE](https://codepen.io/iqq800/pen/QwNWrzE)

## 📁 Project Structure

```
draggable-bottom-sheet-touch-enabled/
├── src/
│   ├── index.html          # Main HTML structure
│   ├── style.css           # Complete styling with responsive design
│   └── script.js           # JavaScript functionality and event handling
├── dist/                   # Distribution files (same as src)
├── LICENSE.txt             # MIT License
└── README.md               # This file
```

## 🛠️ How to Use

### Basic Implementation

1. **Include the HTML structure** in your document:

```html
<button class="show-modal">Show Bottom Sheet</button>
<div class="bottom-sheet">
  <div class="sheet-overlay"></div>
  <div class="content">
    <div class="header">
      <div class="drag-icon"><span></span></div>
    </div>
    <div class="body">
      <!-- Your content goes here -->
      <h2>Your Title</h2>
      <p>Your content...</p>
    </div>
  </div>
</div>
```

2. **Add the CSS** styles to your stylesheet or link the CSS file:

```html
<link rel="stylesheet" href="src/style.css">
```

3. **Include the JavaScript** functionality:

```html
<script src="src/script.js"></script>
```

### Customization

The component is highly customizable:

- **Colors**: Modify CSS variables or directly edit colors in `style.css`
- **Snap Points**: Adjust height thresholds in `script.js` (lines 47-51)
- **Animation Speed**: Modify transition durations in `style.css`
- **Content Styling**: Customize `.body` content styles as needed

## 🎮 Interaction Behavior

### Drag Gestures

- **Drag Up**: Increases sheet height
- **Drag Down**: Decreases sheet height
- **Snap Points**: Sheet automatically snaps to:
  - **Hidden** (< 25% viewport height)
  - **Half Screen** (25-75% viewport height, defaults to 50%)
  - **Full Screen** (> 75% viewport height)

### Touch & Mouse Support

The component supports both touch and mouse events:
- **Desktop**: Click and drag with mouse
- **Mobile**: Touch and drag with finger
- **Hybrid**: Works seamlessly on devices with both input types

### Controls

- **Drag Icon**: Click/tap and drag to adjust sheet height
- **Overlay Click**: Click outside the sheet to close
- **Show Button**: Click to open the sheet at 50% height

## 🎨 Styling Features

- **Modern Design**: Clean, minimalist appearance with subtle shadows
- **Drag Indicator**: Visual drag handle with smooth hover effects
- **Smooth Transitions**: CSS transitions for all state changes
- **Fullscreen Optimization**: Border-radius removal in fullscreen mode
- **Mobile Optimization**: Viewport height calculations and touch-friendly sizing

## 🔧 Technical Implementation

### JavaScript Architecture

- **Event-Driven**: Uses modern event listeners for touch and mouse events
- **State Management**: Tracks dragging state and current sheet height
- **Performance**: Optimized with `requestAnimationFrame`-style calculations
- **Accessibility**: Proper ARIA support and keyboard navigation ready

### CSS Features

- **Flexbox Layout**: Modern CSS for flexible positioning
- **CSS Transforms**: Hardware-accelerated animations
- **Viewport Units**: Responsive height calculations using `vh`
- **Scroll Lock**: Body scroll prevention using `:has()` selector

### Browser Support

- ✅ Chrome 88+
- ✅ Firefox 78+
- ✅ Safari 14+
- ✅ Edge 88+
- ✅ Mobile browsers (iOS Safari, Android Chrome)

## 📄 License

This project is licensed under the MIT License. See [LICENSE.txt](LICENSE.txt) for details.

**Original Author**: iqq800 ([CodePen](https://codepen.io/iqq800))
**Forked From**: Original work by [burnaDLX](https://codepen.io/burnaDLX/pen/myVYqqZ)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](../../issues) and submit pull requests.

## 🌟 Acknowledgments

- Original concept and implementation by iqq800
- Forked from the excellent work by burnaDLX
- Inspired by bottom sheet implementations in popular mobile applications

