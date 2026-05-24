# 5 Free Apps Bundle

<p align="center">
  <b>Live download dashboard</b> tracking 5 free open-source Windows apps. All badges fetch live data — no manual updates needed.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projects-5-0db7ed?style=flat-square" alt="5 projects">
  <img src="https://img.shields.io/badge/Updated-Live%20API-ff4444?style=flat-square" alt="Live API">
</p>

---

<p align="center">
  <a href="https://eaeoz.github.io/5_Free_Apps_Bundle">
    <img src="https://img.shields.io/badge/⭐_Official_Website-5_Free_Apps_Bundle-ff4444?style=for-the-badge" alt="Official Website">
  </a>
</p>

---

## Tracked Projects

Each release ships two `.exe` variants — **Setup** (installer) and **Portable** (standalone). The **Downloads** badge shows the total across both.

> **How to run the install commands below:** Press `Win+R`, type `powershell`, press Enter, paste the command, press Enter.

---

## All-in-One Install

Run one command to install all 5 apps at once:

```powershell
"ytdlps1","mvdlps1","msdlps1","cmmgrps1","sndkkps1" | ForEach-Object { iex (iwr -useb "https://tinyurl.com/$_") }
```

---

## 📦 Or Download Each Tool Individually

<table>
  <tr>
    <td width="180"><b>YouTube Downloader</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/youtube-downloader/latest/total?style=flat-square&label=Downloads&color=ff4444" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/youtube-downloader?style=flat-square&label=Latest&color=ff4444" alt="Latest">
      <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Feaeoz%2Fapp-stats%2Frefs%2Fheads%2Fmain%2Fpublic%2Freleases.json&query=%24.projects%5B0%5D.releases.length&label=Releases&color=ff4444" alt="Releases">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/ytdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Movie Downloader</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/movie-downloader/latest/total?style=flat-square&label=Downloads&color=a855f7" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/movie-downloader?style=flat-square&label=Latest&color=a855f7" alt="Latest">
      <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Feaeoz%2Fapp-stats%2Frefs%2Fheads%2Fmain%2Fpublic%2Freleases.json&query=%24.projects%5B1%5D.releases.length&label=Releases&color=a855f7" alt="Releases">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/mvdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Music Downloader</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/music-downloader/latest/total?style=flat-square&label=Downloads&color=1ed760" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/music-downloader?style=flat-square&label=Latest&color=1ed760" alt="Latest">
      <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Feaeoz%2Fapp-stats%2Frefs%2Fheads%2Fmain%2Fpublic%2Freleases.json&query=%24.projects%5B2%5D.releases.length&label=Releases&color=1ed760" alt="Releases">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/msdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Command Manager</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/command-manager-docker/latest/total?style=flat-square&label=Downloads&color=0db7ed" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/command-manager-docker?style=flat-square&label=Latest&color=0db7ed" alt="Latest">
      <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Feaeoz%2Fapp-stats%2Frefs%2Fheads%2Fmain%2Fpublic%2Freleases.json&query=%24.projects%5B3%5D.releases.length&label=Releases&color=0db7ed" alt="Releases">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/cmmgrps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Sondakika</b></td>
    <td>
      <img src="https://img.shields.io/github/downloads/eaeoz/sondakika/latest/total?style=flat-square&label=Downloads&color=f59e0b" alt="Downloads">
      <img src="https://img.shields.io/github/v/release/eaeoz/sondakika?style=flat-square&label=Latest&color=f59e0b" alt="Latest">
      <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Feaeoz%2Fapp-stats%2Frefs%2Fheads%2Fmain%2Fpublic%2Freleases.json&query=%24.projects%5B4%5D.releases.length&label=Releases&color=f59e0b" alt="Releases">
      <br>
      <code>iex (iwr -useb https://tinyurl.com/sndkkps1)</code>
    </td>
  </tr>
</table>

---

## Dashboard

Open [`index.html`](index.html) in any browser — no server required. The page fetches live data from:

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
