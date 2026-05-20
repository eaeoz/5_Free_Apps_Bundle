# 5 Free Apps Bundle

Live download dashboard for 5 free open-source projects. Fetches release data from GitHub API and renders per-repo download stats.

## Tracked Repos

| App | Repo | Accent | Quick Install |
|-----|------|--------|---------------|
| YouTube Downloader | `eaeoz/youtube-downloader` | `#ff4444` | `iex (iwr -useb https://tinyurl.com/ytdlps1)` |
| Movie Downloader | `eaeoz/movie-downloader` | `#a855f7` | `iex (iwr -useb https://tinyurl.com/mvdlps1)` |
| Music Downloader | `eaeoz/music-downloader` | `#1ed760` | `iex (iwr -useb https://tinyurl.com/msdlps1)` |
| Command Manager | `eaeoz/command-manager-docker` | `#0db7ed` | `iex (iwr -useb https://tinyurl.com/cmmgrps1)` |
| Sondakika | `eaeoz/sondakika` | `#f59e0b` | `iex (iwr -useb https://tinyurl.com/sndkkps1)` |

## Per-Repo Display

Each card shows:

- **Owner avatar + name**
- **App icon** (SVG from the `META` map)
- **Total downloads** across all releases
- **Release count** (number of unique release tags with `.exe` assets)
- **Star count** from GitHub
- **Quick Install** command block with one-click copy
- **Latest `.exe` assets** — each row is a clickable link showing file name, size, and download count
- **Link to repository** on GitHub

## Grand Total Header

When multiple repos are tracked, a hero badge displays the **grand total download count** across all projects.

## Usage

Open `index.html` directly in a browser. The page fetches live data from:

```
https://raw.githubusercontent.com/eaeoz/app-stats/main/public/releases.json
```

No build step or local server required.

## Editing

- Edit the `REPOS` array in the HTML `<script>` to add/remove repos.
- Add a corresponding entry in `META` with `label`, `icon` (SVG string), `accent`, and `cmd`.
- If a repo has no `.exe` assets, the card shows "No executables found".
