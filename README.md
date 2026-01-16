# 💪 Workout Journal Pro

An advanced, progressive web app for tracking workouts with intelligent features like progressive overload suggestions, advanced analytics, and haptic feedback. Built as a single-file HTML app with React.

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![React](https://img.shields.io/badge/React-18-61DAFB?logo=react)

## ✨ Features

### 🎯 Core Tracking
- **Custom Workout Programs**: Create and edit your own workout splits
- **Exercise Library**: Pre-loaded with compound and isolation exercises
- **Set Logging**: Track weight, reps, and notes for every set
- **Rest Timer**: Automatic countdown with haptic feedback
- **Session Timer**: Track total workout duration
- **Plate Calculator**: Visual barbell plate calculator

### 📈 Progressive Overload
- **Smart Suggestions**: Auto-calculated weight progression based on last workout
- **Trend Indicators**: Visual arrows showing if you're progressing (↗️), maintaining (➡️), or regressing (↘️)
- **Suggestion Badges**: Tap to instantly apply recommended weights
- **Warmup Calculator**: Auto-generates warmup sets for any working weight

### 📊 Advanced Analytics
- **Volume by Muscle Group**: Weekly breakdown with visual bar charts
- **Best Days Analysis**: Rankings showing which workouts you perform best on
- **Tonnage Trends**: Line charts tracking total volume over time
- **Lift Progress**: Individual exercise charts (max weight & volume)
- **Personal Records**: Automatic 1RM calculations and PR tracking
- **Deload Detection**: Warns when volume drops 2+ weeks in a row

### 🎨 User Experience
- **Toast Notifications**: Smooth, non-intrusive feedback for all actions
- **Haptic Feedback**: Light vibrations on iOS/Android for button presses
- **Set Completion Animation**: Animated checkmark when completing sets
- **Swipe to Delete**: Swipe left on history items to delete
- **Dark Mode**: Full dark theme support
- **Note System**: Add detailed notes to individual sets

### 💾 Data Management
- **CSV Export**: Export all workout data for analysis in Excel/Sheets
- **JSON Import/Export**: Full backup and restore functionality
- **LocalStorage Persistence**: All data stored locally in browser
- **Weight Tracking**: Track bodyweight over time with chart

## 🚀 Quick Start

### Installation

1. **Download** the `workout-journal-pro.html` file
2. **Open** it in any modern web browser (Chrome, Firefox, Safari, Edge)
3. **Add to Home Screen** (optional, for app-like experience):
   - **iOS**: Tap Share → Add to Home Screen
   - **Android**: Tap Menu → Add to Home Screen

That's it! No installation, no dependencies, no build process.

## 📱 Usage Guide

### Creating Your First Workout

1. Tap the **User** icon (top left)
2. Go to **Schedule Editor**
3. Add a new day (e.g., "Monday")
4. Add exercises with the **+ Add Exercise** button

### Logging a Workout

1. Tap **Start New Session** on the home screen
2. Select your workout day
3. For each exercise:
   - Tap the **suggestion badge** (+5lbs) to apply progressive overload
   - Enter **reps** and **weight** for each set
   - Tap the set number to mark it complete (triggers rest timer)
   - Add **notes** with the 📝 icon if needed
4. Tap **Complete Workout** when done

### Using Progressive Overload

The app automatically suggests weight increases based on your last workout:
- **Green badge** shows suggested weight increase
- **Arrows** (↗️↘️➡️) show your trend
- **Tap the badge** to auto-fill the suggested weight

### Viewing Analytics

Navigate to the **Stats** tab:
- **Volume**: See this week's volume by muscle group
- **Best Days**: Find which workouts you excel at
- **Tonnage**: Track total volume trends over 20 workouts
- **Lift Progress**: Individual exercise progression charts

### Exporting Data

1. Go to **Manage** tab
2. Tap **Export CSV**
3. Open in Excel/Google Sheets for custom analysis

Columns: Date, Day, Exercise, Set, Weight, Reps, Volume, Notes

## 🎨 Customization

### Default Workout Program

The app comes with a 4-day Upper/Lower split:
- **Monday**: Upper Push (Chest, Shoulders, Triceps)
- **Tuesday**: Lower (Quads, Hamstrings, Glutes)
- **Thursday**: Upper Pull (Back, Biceps)
- **Friday**: Lower (Quads, Hamstrings, Glutes)

### Editing Workouts

You can fully customize:
- Day names
- Exercise names and order
- Number of sets
- Rep ranges
- Rest periods
- Form cues/descriptions

### Muscle Group Tracking

Workouts are tagged with muscle groups for volume analytics:
- chest, shoulders, triceps
- back, biceps
- quads, hamstrings, glutes

## 🛠️ Technical Details

### Technologies
- **React 18**: UI framework
- **Babel Standalone**: JSX compilation
- **LocalStorage API**: Data persistence
- **Vibration API**: Haptic feedback
- **Canvas Confetti**: PR celebrations
- **Google Fonts**: Exo 2 font family

### Browser Compatibility
- ✅ Chrome/Edge (88+)
- ✅ Firefox (85+)
- ✅ Safari (14+)
- ✅ Mobile browsers (iOS Safari, Chrome Android)

### Data Storage
All data is stored locally in your browser's LocalStorage:
- `workouts`: Completed workout logs
- `customWorkouts`: Your workout templates
- `measurements`: Bodyweight entries
- `personal-records`: PR calculations
- `dark-mode`: Theme preference

### File Size
- **Single HTML file**: ~110KB
- **No external dependencies** (CDN resources loaded at runtime)
- **Works offline** after first load

## 📊 Data Structure

### Workout Log Entry
```json
{
  "2025-01-15": {
    "day": "monday",
    "exercises": [
      {
        "name": "Flat Barbell Bench Press",
        "logs": [
          {"reps": "8", "weight": "225", "note": "felt strong"},
          {"reps": "8", "weight": "225", "note": ""}
        ]
      }
    ],
    "tonnage": 12500,
    "duration": 3600,
    "completed": true
  }
}
```

## 🎯 Roadmap

### Planned Features
- [ ] Cloud sync (optional)
- [ ] Exercise video library
- [ ] Advanced rest timer (custom intervals)
- [ ] Workout templates/sharing
- [ ] Voice logging ("225 for 8")
- [ ] Apple Health / Google Fit integration
- [ ] Supersets and drop sets
- [ ] Training max calculator
- [ ] Volume landmarks (10k club, etc.)

## 🤝 Contributing

Contributions welcome! This is a single-file app, so:

1. Fork the repository
2. Make your changes to `workout-journal-pro.html`
3. Test in multiple browsers
4. Submit a pull request

### Development Notes
- Keep it as a single file for easy deployment
- Maintain React patterns and component structure
- Add comments for complex logic
- Test on mobile devices
- Keep file size reasonable (<200KB)

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

## 🙏 Credits

Created with ❤️ for the lifting community.

**Fonts**: Exo 2 by Google Fonts  
**Icons**: Custom SVG set  
**Inspiration**: Years of tracking workouts in spreadsheets

## 💬 Support

- **Issues**: Use GitHub Issues for bugs
- **Questions**: Start a Discussion
- **Feature Requests**: Open an Issue with [Feature Request] tag

## 🔒 Privacy

This app:
- ✅ Runs entirely in your browser
- ✅ Stores all data locally
- ✅ Makes **no external API calls** (except CDN resources)
- ✅ Collects **zero analytics**
- ✅ Requires **no account or login**

Your data never leaves your device unless you explicitly export it.

---

**Made with** 💪 **by lifters, for lifters**

[⬆ Back to top](#-workout-journal-pro)
