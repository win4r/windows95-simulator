# Windows 95 Simulator - Development Notes

## Project Structure
- `windows95-simulator.html` - Main application (single-file implementation)
- `README.md` - Project documentation
- `LICENSE` - MIT license

## Technical Architecture

### WindowManager Class
Core system management class that handles:
- Window lifecycle (create, activate, minimize, maximize, close)
- Z-index management for proper layering
- Taskbar integration
- Drag and drop functionality

### Application Framework
Each application follows this pattern:
```javascript
createAppWindow() {
    return {
        title: 'App Title',
        appName: 'app-id', 
        width: 400,
        height: 300,
        content: '<div>App content</div>',
        init: (window) => {
            // App-specific initialization
        }
    };
}
```

### CSS Architecture
- CSS custom properties for Win95 theme colors
- Modular component styling
- Responsive design considerations

## Development Guidelines

### Adding New Applications
1. Create app configuration in `createWindow()` switch statement
2. Implement app-specific HTML content
3. Add initialization logic in `init` function
4. Update start menu if needed

### Styling Guidelines
- Use CSS custom properties for colors
- Follow Win95 visual conventions (2px borders, inset/outset effects)
- Maintain pixel-perfect accuracy where possible

### Browser Testing
Test across:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Performance Considerations
- Minimize DOM manipulations
- Use event delegation where possible
- Implement proper cleanup for closed windows
- Optimize CSS for smooth animations

## Future Enhancements
- Context menus
- Window resizing
- More applications
- Sound effects
- File system simulation