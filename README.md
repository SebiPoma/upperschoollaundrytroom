# UpperSchool Laundry Room

A modern, real-time laundry machine status dashboard for tracking washer and dryer usage in your school's laundry room.

## Features

✨ **Real-Time Status Tracking**
- Monitor 4 washers and 6 dryers simultaneously
- Live countdown timers for active loads
- Color-coded status indicators (free, running, done)

📝 **Easy Machine Management**
- Quick start interface with modal form
- Custom duration and temperature settings
- Duration presets for quick selection
- Clear machines when done

📊 **Activity Insights**
- Real-time activity log of all machine operations
- Completed loads history with detailed information
- Track who used which machine and when

🎨 **Modern UI**
- Dark theme with sleek design
- Fully responsive (mobile, tablet, desktop)
- Smooth animations and transitions
- Grid-based machine layout

## How to Use

### Starting a Load
1. Click on any free machine card
2. Enter your name or room number
3. Select duration (use presets or custom time)
4. Choose wash/heat temperature
5. Click "Start load"

### Clearing a Machine
1. Click the red "Clear" button on an active machine
2. The load is automatically logged to completed history

### Monitoring Progress
- **Live Timer**: Shows remaining time in MM:SS format
- **Progress Bar**: Visual representation of load progress
- **Status Badge**: Shows current machine state (free/running/done)

## Installation

### Option 1: Use Online (Recommended)
Visit: https://sebipoma.github.io/upperschoollaundrytroom/

### Option 2: Run Locally
1. Download `index.html`
2. Double-click to open in your browser
3. Works completely offline

### Option 3: Self-Host
1. Clone this repository
2. Deploy to any static hosting (GitHub Pages, Netlify, Vercel, etc.)
3. No backend required - fully client-side

## Technical Details

- **Built with**: HTML5, CSS3, Vanilla JavaScript
- **No dependencies**: Completely self-contained
- **Browser support**: All modern browsers (Chrome, Firefox, Safari, Edge)
- **Data storage**: Session-based (clears on page refresh)

## Customization

### Change Machine Count
Edit the array lengths in the JavaScript:
```javascript
// For washers:
Array.from({length: 4}, ...)  // Change 4 to desired number

// For dryers:
Array.from({length: 6}, ...)  // Change 6 to desired number
```

### Adjust Durations
Modify `DEFAULTS`:
```javascript
const DEFAULTS = { washer: 35, dryer: 45 };
```

### Change Temperature Options
Update the arrays:
```javascript
const WASHER_TEMPS = ['Cold', 'Cool', 'Warm', 'Hot'];
const DRYER_TEMPS = ['Air Dry / No Heat', 'Low Heat', 'Medium Heat', 'High Heat'];
```

## Features Demo

### Machine States
- 🟦 **Free** - Available for use
- 🟪 **Running** - Currently in use (blue border)
- 🟩 **Done** - Load completed (green border)

### Statistics Bar
Shows real-time counts:
- Active loads running
- Machines ready to grab
- Available washers
- Available dryers

### Activity Log
Tracks all events:
- Load starts with temperature and duration
- Early machine clears
- Completed load times

### Completed Loads Table
Maintains history of:
- Time completed
- User name/room
- Machine ID and type
- Temperature/heat setting

## Tips

💡 **Best Practices**
- Always enter a name so others know who's using the machine
- Use presets for faster load starting
- Check the "ready to grab" status for completed loads
- Clear machines promptly after loads finish

## Future Enhancements

Potential features to add:
- ⏰ Notifications when loads are done
- 💾 Persistent data storage (LocalStorage/Database)
- 📱 Push notifications
- 🔔 Sound alerts
- 📊 Usage statistics and analytics
- 🔐 User authentication
- 📧 Email notifications

## License

MIT License - Feel free to use and modify for your school

## Support

For issues, questions, or suggestions, please create an issue on GitHub.

---

**Created for UpperSchool Students** | Manage your laundry efficiently! 🧺
