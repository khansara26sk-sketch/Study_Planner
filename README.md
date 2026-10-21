# Study Planner

A single-file personal study planner. No build step, no dependencies.

## Run
Open `index.html` in a browser (double-click it), or serve the folder:
    python3 -m http.server 8000   # then visit http://localhost:8000

## Data
- Starts empty. Nothing is pre-filled.
- Saved in your browser's localStorage, so it stays on that browser and device.
- Settings > Export JSON (download) saves a backup file; Copy JSON copies it; Import JSON validates the file, asks for confirmation, and keeps a safety copy of your current data first.
- If stored data is ever unreadable, a copy is kept under the key studyplanner.v1.corrupt.<time> and nothing is deleted.
- Open the site in the same address every time. GitHub Pages sites under the same username share one storage area, and a different address (localhost, a custom domain, the claude.ai preview) has its own separate data. Use Export/Import to move data between addresses.
- Clearing browser data deletes your planner data, so export backups regularly.

## Sections
Dashboard, Study Planner, Subjects, LeetCode Tracker, LeetCode Daily, Daily Streak, Study Timer, Revision Center, Notes, Calendar, Analytics, Settings.

## Not included
Supabase/cloud sync and login, rich-text notes, Pomodoro mode, CSV export, week/day calendar views.

## LeetCode Tracker sections
Buttons above the list filter by current status: All, Solved, Solved Independently, With Hint, With Solution, Needs Revision, TLE, Wrong Answer, Runtime Error, Attempted / In Progress, To Do. Each shows its count.
