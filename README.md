# Innocent-tracker-Innocent's Loan Tracker
A mobile-friendly, installable loan-tracking app. Logs approved/rejected applications, disbursements, targets, and daily reflections — all stored locally on the device (no backend, no account needed).
Files
index.html — the app itself
manifest.json — makes the app installable to a phone home screen
sw.js — service worker, lets the app open even with no signal
icon.png — home-screen / browser-tab icon
All four files must sit in the same folder for install and offline mode to work.
Features
✅ Daily log — track approved & rejected loan applications by date
💸 Disbursement tracker — log loans disbursed, mark withdrawals, add comments
📊 Weekly & monthly stats — approval rates, averages, and breakdowns
🎯 Targets — set daily, weekly, and monthly goals with progress bars
📓 Journal — daily reflections (wins, challenges, improvements, ideas)
🔔 Reminders — set daily alert times to prompt logging
🔥 Streak tracker — consecutive-day logging streak with milestone celebrations
😊 Mood picker — log how each day is going alongside your entry
📴 Works offline — fully functional with no internet after first load
Put it on GitHub Pages
Create a new GitHub repository (public, since Pages needs public for free accounts).
Upload all four files (index.html, manifest.json, sw.js, icon.png) to the root of the repo.
Go to Settings → Pages.
Under "Build and deployment", set Source to "Deploy from a branch".
Pick the main branch and / (root) folder, then Save.
GitHub gives you a link like https://yourusername.github.io/repo-name/ — wait a minute or two after saving for it to go live.
Install it on a phone
iPhone (Safari): open the link → tap the Share icon → Add to Home Screen
Android (Chrome): open the link → tap the menu (⋮) → Add to Home screen / Install app
Once installed it opens full-screen like a normal app, and still works with no internet after the first load.
Updating later
Whenever you upload a new version of index.html (or the other files), open sw.js and bump the version number in this line:
Js
Change it to v2, v3, etc. This tells phones that already installed the app to fetch the new version instead of showing the old cached one.
Data & privacy
Everything (applications, disbursements, journal entries, targets, reminders, moods) is stored in the browser's local storage on the device itself. Nothing is sent anywhere. This also means data does not sync between devices — it stays wherever it was entered. If the browser's data is cleared, or the app is used on a different phone/browser, the history won't carry over.
