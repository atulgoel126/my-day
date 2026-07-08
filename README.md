# My Day — personal daily accountability planner

A single-page web app that walks Atul through the day, block by block, and counts every action completed. Built to run always-on on a plugged-in Android tablet.

**Live:** https://atulgoel126.github.io/my-day/

## Put it on the tablet
1. Open the live link in Chrome on the tablet.
2. Tap **⋮ → Add to Home screen** → it installs as a full-screen app.
3. Open it, tap **Start my day** (this enables alarm sound, keeps the screen awake, and turns on reminders).
4. Keep the tablet plugged in and this app in the foreground.

## ⚠️ Important: set a backup alarm
The in-app 6 AM alarm only rings while the app is open and the screen is on. **Also set a native Clock alarm for 6 AM** as a backstop so a crashed/closed app never means a missed wake. The app then owns the "confirm you're up" check-in and morning checklist.

## Features
- **6 AM confirm-to-dismiss alarm** — snooze 9 min; only stops when you tap "I'm up".
- **Timeline state machine** — the current block is always front and center; tap any block to work on it.
- **Action counter, % done, day streak** — the accountability core.
- **Exercise** — pick trainer / self-exercise / self-walk.
- **Study queue** — 5 courses (~10 sessions each); work the top pending, mark a session, it advances.
- **5 PM reminder** — "30 minutes until no-screen time."
- **Desk-clock mode** (5:30–8:30) — big clock + live report of what's done and still open.
- **LeetCode** placeholder (full module later).
- **Wind-down** checklist + plan tomorrow's meals.
- **Backup** — Settings → Export/Import JSON so your streak is never lost.

## Editing your data
Everything is editable in **⚙️ Settings** (course names) or directly in `index.html` (the `BLOCKS`, `EXERCISE_OPTIONS`, `LEETCODE_LIST` config near the top of the `<script>`). Push a new `index.html` to update the live app.

## Run locally
```
python3 -m http.server 8080
# open http://localhost:8080
```
