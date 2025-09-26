# Windows 95 Desktop Simulator 🖥️

A high-fidelity Windows 95 desktop environment simulator built with pure HTML, CSS, and JavaScript. Experience the nostalgia of the classic 90s operating system right in your web browser!

![Windows 95 Simulator](https://img.shields.io/badge/Windows-95-blue?style=flat-square) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

## 🎯 Features

### ✅ Core Desktop Experience
- **Authentic Win95 UI**: Classic gray theme, 3D borders, and pixel-perfect styling
- **Interactive Taskbar**: Start button, window buttons, and real-time clock
- **Desktop Icons**: My Computer, Recycle Bin, and Notepad shortcuts
- **Start Menu**: Expandable menu with application shortcuts

### 🪟 Window Management System
- **Full Window Controls**: Minimize, maximize/restore, and close buttons
- **Drag & Drop**: Smooth window dragging with boundary detection
- **Z-Index Management**: Proper window layering and activation
- **Taskbar Integration**: Click taskbar buttons to switch or minimize windows

### 📱 Built-in Applications

#### 📝 Notepad
- Full text editing capabilities
- Auto-save to localStorage
- Classic Windows Notepad interface

#### 💻 My Computer
- Browse system drives and folders
- Classic folder view with icons
- Authentic Win95 file explorer layout

#### ⚫ MS-DOS Prompt
Interactive command line with support for:
- `DIR` - List directory contents
- `VER` - Display system version
- `CLS` - Clear screen
- `TIME` - Show current time
- `DATE` - Show current date
- `HELP` - Display available commands

## 🚀 Demo

**[👉 Live Demo - Try it now!](https://your-username.github.io/windows95-simulator)**

Simply open `windows95-simulator.html` in any modern web browser to start using the simulator.

## 🎮 How to Use

### Desktop Interaction
- **Double-click** desktop icons to launch applications
- **Single-click** to select desktop icons
- **Click** the Start button to open the Start menu

### Window Operations
- **Drag** the title bar to move windows
- **Click** minimize (-) to hide windows
- **Click** maximize (□) to toggle fullscreen/windowed mode
- **Click** close (×) to close applications

### Taskbar
- **Click** taskbar buttons to switch between windows
- **Click** active window button to minimize it
- **Real-time clock** displays current time

### Command Prompt
- Type DOS commands and press **Enter** to execute
- Use `HELP` to see available commands
- Use `CLS` to clear the screen

## 🛠️ Technical Implementation

### Architecture
- **Object-Oriented Design**: Clean WindowManager class handling all system operations
- **Modular Applications**: Each app is a self-contained module
- **Event-Driven**: Responsive UI with proper event handling
- **No Dependencies**: Pure vanilla JavaScript, HTML, and CSS

### Key Components
```javascript
class WindowManager {
    // Core system management
    constructor() {
        this.windows = new Map();     // Window instances
        this.zIndex = 100;           // Layer management
        this.activeWindow = null;    // Focus tracking
    }
}
```

### Browser Compatibility
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

## 🎨 Screenshots

### Desktop Environment
![Desktop Screenshot](./screenshots/desktop.png)

### Multiple Windows
![Multiple Windows](./screenshots/windows.png)

### Applications
![Applications](./screenshots/apps.png)

## 📂 Project Structure

```
windows95-simulator/
├── windows95-simulator.html    # Main application file
├── README.md                   # Project documentation
└── screenshots/               # Screenshots for documentation
    ├── desktop.png
    ├── windows.png
    └── apps.png
```

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/windows95-simulator.git
   cd windows95-simulator
   ```

2. **Open the simulator**
   ```bash
   # Simply open the HTML file in your browser
   open windows95-simulator.html
   # or
   python -m http.server 8000  # For local server
   ```

3. **Start exploring!**
   - Double-click desktop icons to launch apps
   - Try the DOS prompt with various commands
   - Experience the authentic Win95 feel

## 🎯 Development Roadmap

### Planned Features
- [ ] Desktop right-click context menu
- [ ] Window resizing handles
- [ ] More built-in applications (Calculator, Paint)
- [ ] File system simulation
- [ ] Sound effects
- [ ] Network simulation (Dial-up connection)
- [ ] Games (Solitaire, Minesweeper)

### Current Limitations
- No file system persistence between sessions
- Limited to simulated DOS commands
- No actual file operations in My Computer

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some amazing feature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

### Areas for Contribution
- 🎨 UI/UX improvements
- 📱 Additional applications
- 🔧 Bug fixes and optimizations
- 📚 Documentation enhancements
- 🎵 Sound effects and animations

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by the original Windows 95 operating system by Microsoft
- Built with love for retro computing enthusiasts
- Thanks to the web development community for inspiration and resources

## 🐛 Known Issues

- Window dragging may be sluggish on older devices
- Some UI elements might not render perfectly on very small screens
- localStorage data persists until manually cleared

## 📞 Support

If you encounter any issues or have questions:
- 🐛 [Report bugs](https://github.com/your-username/windows95-simulator/issues)
- 💡 [Request features](https://github.com/your-username/windows95-simulator/issues)
- 💬 [Start discussions](https://github.com/your-username/windows95-simulator/discussions)

---

<div align="center">
  
**Relive the 90s computing experience! 🎉**

Made with ❤️ by developers who miss the good old days

[⭐ Star this repo](https://github.com/your-username/windows95-simulator) if you enjoyed the nostalgia!

</div>