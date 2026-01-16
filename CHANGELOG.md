# Changelog

All notable changes to Workout Journal Pro will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0] - 2025-01-15

### Added
- **Progressive Overload System**
  - Smart weight suggestions based on last workout
  - Visual trend indicators (↗️↘️➡️)
  - Tap-to-apply suggestion badges
  - Progressive overload algorithm

- **Advanced Analytics**
  - Weekly volume by muscle group with bar charts
  - Best performance days ranking
  - Tonnage trend charts (last 20 workouts)
  - Individual lift progress charts
  - Deload week detection

- **Enhanced UX**
  - Toast notification system (no more alerts!)
  - Haptic feedback throughout app
  - Set completion animations
  - Swipe-to-delete in history
  - Bottom sheet modals for notes
  - Improved touch targets

- **Data Management**
  - CSV export functionality
  - JSON import/export
  - Note system for individual sets
  - Enhanced data visualization

- **Workout Features**
  - Warmup calculator
  - Enhanced plate calculator
  - Session timer with pause
  - Rest timer with custom adjustments
  - Per-set note taking

### Changed
- Complete UI/UX overhaul
- Replaced all alert() calls with toast notifications
- Improved mobile responsiveness
- Better dark mode contrast
- Smoother animations throughout
- Enhanced stat cards and charts

### Fixed
- Touch target sizes on mobile
- Form input zoom issues on iOS
- Dark mode inconsistencies
- Chart rendering on small screens
- LocalStorage edge cases

## [1.0.0] - 2024-12-01

### Added
- Initial release
- Basic workout logging
- Custom workout creation
- Exercise library
- Personal records tracking
- Dark mode
- Weight tracking
- Plate calculator
- History view
- LocalStorage persistence

---

## Version Numbering

- **Major (X.0.0)**: Breaking changes, major feature additions
- **Minor (0.X.0)**: New features, backwards compatible
- **Patch (0.0.X)**: Bug fixes, minor improvements
