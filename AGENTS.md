# AGENTS.md

## Repo overview

Single static HTML dashboard (`youtube-downloader.html`) that fetches GitHub release APIs and renders download stats. `youtube-downloader.json` is a local data snapshot (not consumed by the page).

No build system, package manager, tests, CI, or config files.

## Open / preview

- Open `youtube-downloader.html` directly in a browser (no server needed)
- For live data, the page fetches from `api.github.com` — no local JSON file required

## Adding / editing repos

- Edit the `REPOS` array in the HTML `<script>` — each entry is a `"owner/repo"` string
- Add a matching entry in `META` with `label`, `icon` (SVG string), and `accent` color
- If a repo has no `.exe` assets, the card shows "No executables found"

## Constraints

- The page is intended for CodePen embed — must be fully self-contained (no external JS deps, all CSS inline)
- All `.exe` rows must be clickable links (`browser_download_url` from the API)
- Design must work in a dark theme only
