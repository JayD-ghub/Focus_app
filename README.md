# Focus — Lab Notebook

A focus timer, daily journal, and progress tracker, styled like a physicist's
lab notebook. Built as a single-page installable web app — no account, no
server, no tracking. Everything stays on your device.

## Features

**Timer**
- Pomodoro-style focus/break timer with 25/5, 50/10, and 90/15 presets, or set
  your own custom minutes
- Timestamp-anchored, so it stays accurate even if you lock your phone or
  switch apps mid-session
- "First action" and "done when" fields to set intent before each block

**Journal**
- A free-write entry plus a structured shutdown note (finished today,
  tomorrow's first action, any blockers) for each day
- A full archive: a calendar you can browse month by month, and a recent
  entries list — tap any past day to read or edit it

**Progress**
- Today / week / month / year views
- The year view is a GitHub-style heatmap, colored with the *viridis*
  colormap — deeper focus days shade toward yellow
- Streaks, totals, daily averages, and a one-click JSON backup export/import

**Personal touches**
- Greets you by name (set on first launch, editable anytime in Progress →
  *the researcher*)
- A soft two-tone chime plays when a focus block or break ends (synthesized
  in-browser, no audio file needed) — tap the speaker icon next to the
  greeting to mute it
- Installs to your home screen with an atom icon and opens full-screen, no
  browser bar
- Works offline once installed (via a service worker)

## Files

```
index.html          the app itself (structure, styles, and logic)
manifest.json        makes it installable as a standalone app
service-worker.js    caches the app for offline use
icon-192.png          )
icon-512.png          )  app icons, shown on your home screen
apple-touch-icon.png  )
```

## Getting it live

1. Unzip the folder if you downloaded it as a `.zip`.
2. Create a new **public** GitHub repository.
3. Upload all 6 files (loose, not the zip) and commit.
4. Repo → **Settings → Pages** → Source: *Deploy from a branch*, Branch:
   `main`, folder `/(root)` → Save.
5. Your live link appears at `https://<username>.github.io/<repo-name>/`
   after a minute or two.
6. Open that link on your phone and **Add to Home Screen**.

## A note on your data

Everything — journal entries, sessions, your name — is saved in this
browser's local storage on whichever device you use. It's genuinely
persistent (survives closing the app, restarting your phone, etc.), but
clearing site data would erase it. Use **Progress → export backup**
occasionally to keep a copy, especially before switching devices.
