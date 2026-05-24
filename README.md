# Debt Tracker PWA

A personal debt tracking Progressive Web App. Track debts with flexible installments, mark payments, view your debt-free date, and take notes — all stored locally on your device.

**Live URL:** Replace this after deploying, e.g. `https://your-username.github.io/debt-tracker/`

## Features

- Add, edit, and delete debts with full due dates (day + month + year)
- Mark installments as paid — balances update instantly
- Group by debt type or due date
- Payday warnings (configurable day of month, default 22nd)
- Overdue payment highlighting
- Debt-free date projection
- Local notes
- Works offline after first load (PWA)

## Run Locally

Service workers require HTTP. From this folder:

```bash
python3 -m http.server 8080
```

Open **http://localhost:8080/index.html** in your browser.

## Deploy

Upload the entire `Debt Tracker` folder to any static host with HTTPS:

- [Netlify Drop](https://app.netlify.com/drop) — drag and drop the folder
- [GitHub Pages](https://pages.github.com/)
- [Cloudflare Pages](https://pages.cloudflare.com/)

After deploying, update the **Live URL** line above with your actual URL.

## Add to Home Screen (iPhone)

1. Open the app URL in **Safari** (not Chrome)
2. Tap the **Share** button (square with arrow)
3. Scroll down and tap **Add to Home Screen**
4. Tap **Add**

The app opens full-screen like a native app and keeps your data in local storage.

## Add to Home Screen (Android)

1. Open the app URL in **Chrome**
2. Tap the menu (⋮) → **Install app** or **Add to Home screen**
3. Confirm

## Data & Privacy

All data is stored in your browser's `localStorage`. Nothing is sent to a server. Clear browser data or uninstalling the PWA will delete your data — back up by exporting (future feature) or copying data from browser dev tools if needed.

## Version

Current app version: **1.3.0**

Settings → About shows the installed version. Data migrations run automatically on load via `debt_tracker_version` in localStorage.

