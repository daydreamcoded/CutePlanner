# Egg Planner ♡

A cozy Tamagotchi-inspired planner prototype: pastel egg shell, virtual pet, daily tasks, calendar view, journal, focus timer, and customizable themes.

## Features
- Egg-shaped, responsive interface for desktop and iPad/mobile
- Daily tasks with categories, completion progress, and pet hearts
- Monthly calendar with add/delete events
- Export events as an `.ics` file for Apple Calendar or Google Calendar
- Virtual pet interactions and shell themes
- Journal and Pomodoro-style focus timer
- Export/import planner backup as JSON

## Run locally
Open `index.html` in a modern browser. Planner data is saved in that browser's local storage.

## Publish with GitHub Pages
A GitHub Actions workflow is included in `.github/workflows/pages.yml`. In the repository, open **Settings → Pages** and ensure the source is configured for **GitHub Actions**. The workflow will publish the root site after a push to `main`.

## Calendar integration status
This first web prototype supports local planner events and exporting them as an `.ics` calendar file that can be imported into Apple Calendar or Google Calendar. It does **not** yet have direct account connection or two-way synchronization.

- Google Calendar two-way sync requires a Google Cloud project, OAuth consent configuration, a client ID, and Calendar API authorization.
- Direct Apple Calendar access on iOS requires a native app or wrapper with EventKit permissions. A static GitHub Pages site cannot access EventKit directly.
- Never commit OAuth client secrets or private tokens to this public repository.

## Privacy
Tasks, journal entries, themes, and events stay in this browser's local storage unless the user exports them. This prototype has no account system or cloud sync.
