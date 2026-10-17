JEE TIME TRACKER — ANDROID INSTALLATION

Files included:
- index.html, styles.css, app.js: the app
- manifest.json, sw.js, icons: install/offline support

IMPORTANT:
A PWA needs to be served over HTTPS (or localhost) for installation and service-worker offline support. Opening index.html directly may let the interface run, but it will not provide reliable install/offline functionality.

RECOMMENDED SETUP (GitHub Pages, free):
1. On your computer, unzip this folder.
2. Create a GitHub repository and upload every file in this folder to the repository root.
3. In the repository, open Settings > Pages.
4. Under Build and deployment, choose Deploy from a branch; select the main branch and /(root), then Save.
5. Wait for GitHub Pages to publish the site. Open the HTTPS URL it gives you.
6. On your Android phone, open that URL in Chrome.
7. Chrome menu (three dots) > Install app or Add to Home screen. The wording can vary.
8. Open the installed app. Use Settings / browser permissions to allow notifications if desired.

LOCAL DATA:
- Logs are stored in localStorage on that browser/device. They are not uploaded to a server by this app.
- Browser data clearing, uninstalling, or using a different browser/profile may remove or separate the logs.
- Use Weekly stats > Export backup (JSON) regularly. Use Import backup to restore.
- The app does not sync automatically between devices.

ALARMS LIMITATION:
Web notifications and JavaScript timers are best-effort. Android battery optimization, browser suspension, and app closure can delay or suppress alarms. For alarms that must never be missed, also set Android Clock alarms. This app checks missed blocks while open; background checks can be delayed. It is not a replacement for a native alarm app.

TIME ACCOUNTING:
- Study timer counts active running time only. Paused time is excluded.
- Finish & log saves whole focused minutes; sub-minute time is rounded down.
- Quick log adds manually entered focused minutes.
- Interruption minutes are tracked separately in the daily log and are not automatically subtracted from entries, so do not subtract them twice.
- Accuracy = correct answers / attempted questions. If a session has no question data, it does not affect accuracy.
- Streak counts consecutive calendar days with at least one logged focused minute, starting today and moving backward.
- Missed timetable blocks are evaluated while the app is open. Mark each missed block done or skipped to keep the log accurate.

PRIVACY:
No analytics, account, or external data service is included in the app. Hosting the static files serves the app code, but study logs remain in the browser storage on your device.
