# Central Coast & Sydney Family Holiday Planner

A mobile-friendly family holiday event website covering **11 December 2026 to 5 January 2027**.

## Publish to GitHub Pages

1. Use this public repository `natchilazarus/dec26`.
2. Site files live at the repository root (`index.html`, `events.json` and `.nojekyll`).
3. Open the repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select the default branch (usually `main`), choose **/ (root)**, and **Save**.
5. Once GitHub Pages finishes deploying, open the **Visit site** link shown in Settings → Pages.

For a normal project repository, the URL is usually `https://<github-username>.github.io/<repo-name>/`.

If you want to place this inside an existing project rather than its root, use a top-level `docs/` folder containing all three files and select `/docs` as your Pages source.

## How daily updates work

The page loads current listings from `events.json` each time it is opened or refreshed. That means you can update the event database **without editing HTML**:

1. Open `events.json` in GitHub.
2. Click the pencil icon (**Edit this file**).
3. Update existing records, add event objects, or mark event statuses. Each event needs a stable unique `id` and values matching the existing field names.
4. Change `last_verified` (ISO date format: `YYYY-MM-DD`) and append the day's corrections/additions in `change_log`.
5. Commit the change. Refresh the website to see the new content.

**Important:** The ChatGPT 9 AM event research task is being linked to this repository through its GitHub connector. Automatic website data updates are confirmed only after the task writes `events.json` and the published page reflects its new version; until then, edits can be made directly in GitHub.

## Features and limitations

- Text search, region/category/date filters, event status flags and booking/official information links.
- Family favourites are stored separately in each browser using local storage. Favourites **do not sync across devices**.
- Free static hosting on GitHub Pages for an eligible repository.
- This is a public website; do not place private family data or credentials in the files.
- Event schedules and prices can change: follow the linked organizer/ticketing page before booking.
- Date/status labels indicate what the event directory recorded at verification time, not a real-time ticket availability guarantee.