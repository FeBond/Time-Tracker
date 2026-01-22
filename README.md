# ⏱️ Time Tracker App

A simple, elegant web application for tracking your work hours with multiple entries per day. Features include a stopwatch, per-entry timers, dark mode, and data backup/restore functionality.

## 📋 Features

- **Stopwatch**: Main stopwatch that auto-fills entry forms
- **Multiple Time Periods**: Track multiple start/stop times for each entry
- **Per-Entry Timers**: Each entry has its own timer with pause/resume
- **Today's Summary**: Quick view of today's total time and entries
- **All Entries**: View and filter all historical entries
- **Dark Mode**: Toggle between light and dark themes
- **Data Backup**: Export and import your data as JSON files
- **Second-Level Precision**: Tracks time down to the second

## 🚀 Getting Started

### Option 1: Open Directly in Browser

1. Download all files (`index.html`, `styles.css`, `app.js`, and `README.md`)
2. Keep all files in the same folder
3. Double-click `index.html` to open it in your default browser
   - Or right-click `index.html` → "Open With" → Choose your browser

### Option 2: Use a Local Web Server (Recommended)

For the best experience, use a local web server:

**Using Python:**
```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```
Then open: `http://localhost:8000`

**Using Node.js (http-server):**
```bash
npx http-server
```

**Using VS Code:**
- Install the "Live Server" extension
- Right-click `index.html` → "Open with Live Server"

### Option 3: Open on iPhone/iPad (Safari)

iOS Safari does not reliably open local `file://` HTML files. The most dependable way is to serve the files from your computer and open them over your local Wi‑Fi network.

1. On your computer, run a local web server in the project folder:
   ```bash
   python3 -m http.server 8000
   ```
2. Find your computer's local IP address (example: `192.168.1.25`).
3. On your iPhone/iPad (same Wi‑Fi), open Safari and go to:
   `http://<your-ip>:8000`

### Option 4: Host It Once (GitHub Pages / Netlify)

This app is a static site (HTML/CSS/JS), so you can host it for free and open it from any device.

**GitHub Pages (free for public repos):**
1. Create a new public GitHub repository.
2. Upload `index.html`, `styles.css`, and `app.js`.
3. Go to **Settings → Pages** and enable Pages on the `main` branch.
4. Open the provided URL on your phone.

**Netlify (free tier):**
1. Create a Netlify account.
2. Drag and drop the folder containing `index.html`, `styles.css`, and `app.js`.
3. Open the provided URL on your phone.

## 📖 How to Use

### Creating an Entry

1. **Manual Entry:**
   - Select a date
   - Enter a description (optional)
   - Add start and end times
   - Click "Add Another Period" to track multiple time blocks
   - Click "Add Entry"

2. **Using the Stopwatch:**
   - Click "Start" to begin tracking
   - The stopwatch will create an entry automatically
   - Enter a description while it's running
   - Click "Stop" to finalize the entry

### Managing Entries

- **View Today's Entries**: Check the "Today's Summary" section
- **View All Entries**: Scroll to "All Entries" section
- **Edit an Entry**: Click "Edit" on any entry in the "All Entries" section
- **Delete an Entry**: Click "Delete" on any entry
- **Use Entry Timer**: Each entry has its own timer - click "Start Timer" to track additional time

### Backup & Restore

- **Export Data**: Click "💾 Export" in the header to download a backup file
- **Import Data**: Click "📥 Import" in the header and select a backup JSON file
- **Important**: Back up regularly! Data is stored in your browser's local storage

## 💾 Data Storage

- All data is stored locally in your browser using **localStorage**
- Data persists until you clear browser data
- Each browser/device has its own separate data
- Use the Export feature to back up your data regularly

## 🌙 Dark Mode

Click the moon/sun icon in the header to toggle dark mode. Your preference is saved automatically.

## 📁 File Structure

```
Time Tracker App/
├── index.html      # Main HTML file
├── styles.css      # Styling and dark mode
├── app.js          # Application logic
└── README.md       # This file
```

## ⚠️ Important Notes

- **Browser Compatibility**: Works best in modern browsers (Chrome, Firefox, Safari, Edge)
- **Data Storage**: Data is stored locally - clearing browser data will delete your entries
- **No Internet Required**: This app works completely offline
- **Privacy**: All data stays on your device - nothing is sent to any server

## 🐛 Troubleshooting

**App not working?**
- Make sure all files are in the same folder
- Try using a local web server instead of opening the file directly
- Check browser console for errors (F12 → Console)

**Data disappeared?**
- Check if you cleared browser data
- Try importing from a backup file if you have one
- Data is stored per browser/device

**Can't see entries?**
- Check the "All Entries" section
- Use "Show All" to clear any filters
- Make sure entries were saved (check browser console)

**iPhone Safari won't open the HTML file?**
- iOS blocks or limits local `file://` pages
- Use the "Local Web Server" steps above and open the site via Wi‑Fi

**Want to host it once and forget it?**
- Use the GitHub Pages or Netlify steps above

## 📝 Version

Version 1.0 - December 2024

## 📄 License

Free to use and share!

---

**Enjoy tracking your time!** ⏱️

