# Contributing to Workout Journal Pro

First off, thanks for taking the time to contribute! 🎉💪

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates.

When creating a bug report, include:
- **Clear title and description**
- **Steps to reproduce** the behavior
- **Expected behavior**
- **Screenshots** if applicable
- **Browser and OS** information
- **Any error messages** from the console

### Suggesting Features

Feature requests are welcome! Please:
- Check if the feature already exists
- Explain the use case
- Consider how it fits with existing features
- Be specific about the desired behavior

### Pull Requests

1. **Fork** the repository
2. **Create a branch** for your feature (`git checkout -b feature/AmazingFeature`)
3. **Make your changes** to `workout-journal-pro.html`
4. **Test thoroughly**:
   - Test in Chrome, Firefox, Safari
   - Test on mobile (iOS and Android if possible)
   - Test dark mode
   - Test data persistence (refresh page)
5. **Commit** with a descriptive message
6. **Push** to your fork
7. **Open a Pull Request**

### Development Guidelines

#### Architecture
- This is a **single-file HTML app** - keep it that way!
- All React components are in the `<script type="text/babel">` section
- CSS is in the `<style>` section
- No external dependencies beyond CDN resources

#### Code Style
- Use **functional React components** with hooks
- Keep components **small and focused**
- Use **meaningful variable names**
- Add **comments** for complex logic
- Follow existing **formatting patterns**

#### React Patterns
```javascript
// ✅ Good - Functional component with hooks
function MyComponent() {
  const [state, setState] = useState(initial);
  
  useEffect(() => {
    // side effects
  }, [dependencies]);
  
  return <div>...</div>;
}

// ❌ Avoid - Class components
class MyComponent extends React.Component { ... }
```

#### State Management
```javascript
// ✅ Good - Use Context for global state
const { showToast } = React.useContext(ToastContext);

// ✅ Good - Local state for component-specific data
const [expanded, setExpanded] = useState(false);

// ❌ Avoid - Prop drilling through many levels
```

#### Styling
```css
/* ✅ Good - Use CSS variables */
.card {
  background: var(--bg-secondary);
  color: var(--text-primary);
}

/* ✅ Good - Mobile-first responsive */
.element {
  padding: 16px;
}
@media (min-width: 768px) {
  .element { padding: 24px; }
}

/* ❌ Avoid - Hardcoded colors */
.card {
  background: #ffffff;
  color: #000000;
}
```

#### Testing Checklist

Before submitting a PR, test:

**Functionality**
- [ ] Feature works as intended
- [ ] No console errors
- [ ] Data persists after page refresh
- [ ] Export/import still works

**Cross-Browser**
- [ ] Chrome/Edge (latest)
- [ ] Firefox (latest)
- [ ] Safari (latest)
- [ ] Mobile Safari (iOS)
- [ ] Chrome Android

**Responsive Design**
- [ ] Works on phone (375px width)
- [ ] Works on tablet (768px width)
- [ ] Works on desktop (1920px width)
- [ ] Touch targets are 44x44px minimum

**Accessibility**
- [ ] Forms are keyboard navigable
- [ ] Buttons have proper labels
- [ ] Color contrast meets WCAG standards
- [ ] Works with dark mode

**Performance**
- [ ] File size under 200KB
- [ ] No significant lag on interactions
- [ ] Charts render smoothly

### What to Contribute

**High Priority**
- Bug fixes
- Mobile UX improvements
- Performance optimizations
- Accessibility improvements
- Dark mode refinements

**Medium Priority**
- New chart types
- Additional analytics
- UI polish
- New workout templates

**Nice to Have**
- Advanced features (supersets, etc.)
- Integrations (Health apps)
- Workout sharing

## Questions?

- Open an **Issue** for bugs or features
- Start a **Discussion** for general questions
- Comment on existing **PRs** if relevant

## Recognition

Contributors will be added to:
- README.md credits section
- GitHub contributors page

Thank you for making Workout Journal Pro better! 💪

---

**Remember**: The goal is to create the best workout tracking experience while keeping the app simple, fast, and dependency-free.
