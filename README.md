# Pure Bodybuilding Workout Tracker

A comprehensive web application for tracking the Pure Bodybuilding Upper/Lower Split Program by Jeff Nippard. This single-file HTML application provides everything you need to track your workouts, monitor progress, and stay motivated.

## 🚀 Features

### Core Functionality
- **10-Week Program Structure**: Complete upper/lower split program with 5 workout days per week
- **Exercise Tracking**: Log weights and reps for every set
- **Video Demonstrations**: Direct YouTube links to exercise form videos (158 exercises included)
- **Progress Tracking**: Automatic calculation of completed workouts, total volume, and workout streaks
- **Rest Timer**: Built-in timer with quick presets (30s, 60s, 90s, 2m, 3m)
- **Data Persistence**: All data saved locally in your browser

### Workout Features
- **General Warm-Up Protocol**: Guided warm-up with video demonstrations
- **Exercise Details**: Shows warm-up sets, working sets, rep ranges, and intensity techniques
- **Visual Progress Indicators**: Completed exercises and days marked with checkmarks
- **Set Completion**: One-click set completion with automatic rest timer activation

### Additional Features
- **Progress Dashboard**: View total workouts completed, volume lifted, and current streak
- **Workout History**: Table view of recent completed sets with date, exercise, weight, and reps
- **Notes Section**: Keep track of thoughts, goals, and observations
- **Data Export/Import**: Backup your progress or transfer between devices
- **Mobile Responsive**: Optimized for use during workouts on any device

## 📱 How to Use

### Getting Started
1. Download the `workout-tracker.html` file
2. Open it in any modern web browser (Chrome, Firefox, Safari, Edge)
3. No installation or server required - it runs entirely in your browser

### During Your Workout
1. Select your current week (Week 1-10)
2. Choose your workout day (Upper #1, Lower #1, Upper #2, Lower #2, Arms & Weak Points)
3. Complete the general warm-up exercises
4. For each exercise:
   - Watch the video demonstration if needed
   - Enter weight and reps for each set
   - Click "Complete" when done (starts rest timer automatically)
   - Move to the next set after your rest period

### Tracking Progress
- **Progress Tab**: View your statistics and trends
- **History Tab**: See your recent workout history
- **Notes Tab**: Keep workout notes and observations

### Data Management
- **Export**: Save your workout data as a JSON file for backup
- **Import**: Restore your data from a previously exported file
- All data is automatically saved in your browser's local storage

## 🎯 Program Structure

### Weekly Schedule
- **Upper #1**: Shoulders, lats, chest, back, triceps focus
- **Lower #1**: Hamstrings, adductors, quads, calves
- **Upper #2**: Back, shoulders, lats, chest, biceps
- **Lower #2**: Hamstrings, quads, glutes, calves
- **Arms & Weak Points**: Customizable weak point training + arms

### Intensity Techniques
The program includes various intensity techniques:
- Myo-reps
- Long-length Partials
- Dropsets
- Mechanical Dropsets
- Static Stretches
- Integrated Partials

## 💾 Data Storage

All workout data is stored locally in your browser using localStorage. This means:
- Your data persists between sessions
- No account or login required
- Complete privacy - your data never leaves your device
- Clear browser data will remove your workout history

## 🔄 Backup Recommendations

To prevent data loss:
1. Regularly export your data using the Export button
2. Save the JSON file in a safe location
3. You can import this file if you switch devices or browsers

## 📊 GitHub Deployment

To host this on GitHub Pages:
1. Create a new repository
2. Upload the `workout-tracker.html` file
3. Rename it to `index.html`
4. Enable GitHub Pages in repository settings
5. Access your tracker at: `https://[your-username].github.io/[repository-name]`

## 🛠️ Technical Details

- **Framework**: React 18 (loaded via CDN)
- **Charts**: Chart.js for progress visualization
- **Storage**: Browser localStorage API
- **Styling**: Custom CSS with mobile-responsive design
- **No Dependencies**: Single HTML file, no build process required

## 📝 License

This tracker is for personal use with the Pure Bodybuilding program by Jeff Nippard. Please purchase the official program to access the complete training methodology and instructions.

## 🤝 Contributing

Feel free to fork this repository and customize the tracker for your needs. Some ideas for enhancements:
- Add 1RM calculators
- Include nutrition tracking
- Add social features for workout partners
- Integrate with fitness APIs
- Add progressive overload recommendations

## 🐛 Troubleshooting

**Data not saving?**
- Check if your browser allows localStorage
- Try a different browser if issues persist

**Videos not loading?**
- Ensure you have an internet connection
- YouTube links open in a new tab

**Timer not working?**
- Refresh the page
- Check browser permissions for background timers

## 📧 Support

For issues or questions about the tracker, please open an issue on GitHub.
For questions about the workout program itself, please refer to the official Pure Bodybuilding documentation.

---

**Note**: This is an unofficial tracker created for personal use. All workout programming and exercise selection credit goes to Jeff Nippard and the Pure Bodybuilding program.