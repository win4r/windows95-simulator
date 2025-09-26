# Contributing to Windows 95 Simulator 🚀

Thank you for your interest in contributing to the Windows 95 Simulator! This document provides guidelines and information for contributors.

## 🎯 How to Contribute

### Reporting Bugs 🐛
- Use the bug report template in GitHub Issues
- Include browser version, OS, and steps to reproduce
- Provide console errors if available

### Suggesting Features 💡
- Use the feature request template in GitHub Issues
- Explain the use case and expected behavior
- Consider if the feature fits the Win95 aesthetic

### Code Contributions 💻

#### Prerequisites
- Modern web browser for testing
- Basic knowledge of HTML, CSS, and JavaScript
- Familiarity with Win95 UI conventions

#### Development Setup
1. Fork the repository
2. Clone your fork locally
3. Open `windows95-simulator.html` in a browser
4. Make your changes
5. Test across different browsers

#### Pull Request Process
1. Create a feature branch: `git checkout -b feature/amazing-feature`
2. Make your changes with clear, descriptive commits
3. Test thoroughly across browsers
4. Update documentation if needed
5. Submit a pull request with detailed description

## 🎨 Coding Standards

### HTML
- Use semantic HTML where possible
- Maintain clean, readable structure
- Follow existing indentation style

### CSS
- Use CSS custom properties for theming
- Follow BEM-like naming conventions
- Maintain Win95 visual authenticity
- Ensure responsive design

### JavaScript
- Use modern ES6+ features
- Follow existing code style and patterns
- Add comments for complex logic
- Handle errors gracefully
- Use meaningful variable names

### Win95 Design Principles
- Maintain the classic gray color scheme (#c0c0c0)
- Use 2px outset/inset borders for 3D effects
- Follow Win95 font conventions (MS Sans Serif, 11px)
- Keep icons simple (emoji or Unicode symbols)
- Respect the retro aesthetic

## 🏗️ Architecture Guidelines

### Adding New Applications
1. Create app config in WindowManager
2. Follow the established app pattern:
   ```javascript
   createAppWindow() {
       return {
           title: 'App Title',
           appName: 'unique-id',
           width: 400,
           height: 300,
           content: '<div>App HTML</div>',
           init: (window) => {
               // App initialization
           }
       };
   }
   ```
3. Add to start menu if appropriate
4. Test window operations (drag, minimize, maximize, close)

### Window Management
- All windows should be draggable
- Implement proper z-index management
- Support taskbar integration
- Handle window boundaries

### Performance Considerations
- Minimize DOM queries
- Use event delegation
- Clean up event listeners
- Optimize CSS animations

## 🧪 Testing

### Manual Testing Checklist
- [ ] Desktop icons respond to clicks and double-clicks
- [ ] Windows can be dragged, minimized, maximized, and closed
- [ ] Taskbar buttons function correctly
- [ ] Start menu opens and closes properly
- [ ] Applications load and function as expected
- [ ] No console errors
- [ ] Works across different screen sizes

### Browser Compatibility
Test on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Responsive Testing
- Desktop (1920×1080, 1366×768)
- Tablet (1024×768, 768×1024)
- Mobile (375×667, 414×896)

## 📝 Documentation

### Code Documentation
- Add JSDoc comments for complex functions
- Document any Win95-specific behavior
- Explain non-obvious design decisions

### User Documentation
- Update README.md for new features
- Include screenshots if UI changes
- Update feature lists and compatibility info

### Development Documentation
- Update DEVELOPMENT.md for architecture changes
- Document new patterns or conventions
- Include troubleshooting information

## 🎯 Priority Areas for Contribution

### High Priority
- 🐛 Bug fixes and stability improvements
- 📱 Mobile/tablet responsiveness
- ♿ Accessibility improvements
- 🔧 Performance optimizations

### Medium Priority
- 🎨 New applications (Calculator, Paint, Games)
- 📁 File system simulation
- 🖱️ Right-click context menus
- 🔧 Window resizing functionality

### Low Priority
- 🔊 Sound effects
- 🎮 Easter eggs
- 🌐 Network simulation features
- 🎨 Theme customization

## 📋 Issue Labels

- `bug` - Something isn't working
- `enhancement` - New feature or request
- `good first issue` - Good for newcomers
- `help wanted` - Extra attention needed
- `documentation` - Improvements or additions to docs
- `duplicate` - This issue already exists
- `wontfix` - This will not be worked on

## 🤝 Code of Conduct

### Our Standards
- Be respectful and inclusive
- Focus on constructive feedback
- Help others learn and grow
- Celebrate the retro computing community

### Unacceptable Behavior
- Harassment or discrimination
- Trolling or inflammatory comments
- Personal attacks
- Publishing private information

## 🎉 Recognition

Contributors will be recognized in:
- GitHub contributors section
- Potential mentions in release notes
- Community appreciation posts

## 📞 Getting Help

- 💬 GitHub Discussions for questions
- 🐛 GitHub Issues for bugs
- 📧 Direct contact via repository maintainer

---

Thank you for helping make the Windows 95 Simulator even better! Your contributions help preserve and celebrate computing history. 🖥️✨