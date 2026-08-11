<div align="center">

# 🧩 Optional / Third‑party Widgets

### Extra GitHub Profile README components for users who want a richer, more dynamic profile.

[![Back to README](https://img.shields.io/badge/←_Back_to-README-181717?style=for-the-badge&logo=github)](README.md)
[![Live Preview](https://img.shields.io/badge/👀_Live-Preview-0969da?style=for-the-badge)](LIVE_PREVIEW.md)

</div>

> [!WARNING]
> The widgets on this page depend on external services, APIs, GitHub Actions or user-specific setup. They are **optional** and should not be treated as guaranteed-uptime core components.

> [!TIP]
> Use these only after your basic profile already looks good. Dynamic widgets are best used as enhancements, not as the foundation of your README.

---

## Contents

- [GitHub Trophies](#-github-trophies)
- [Activity Graph](#-activity-graph)
- [Dynamic Quote](#-dynamic-quote)
- [Contribution Snake](#-contribution-snake)
- [Pinned Repository Cards](#-pinned-repository-cards)
- [WakaTime Coding Activity](#️-wakatime-coding-activity)
- [Spotify / Now Playing](#-spotify--now-playing)
- [Discord Presence](#-discord-presence)
- [Visitor Tracking](#-visitor-tracking)
- [Reliability Guide](#️-reliability-guide)

---

# 🏆 GitHub Trophies

GitHub Profile Trophy creates dynamic achievement-style cards from public GitHub activity.

### Code

```md
[![trophy](https://github-profile-trophy.vercel.app/?username=USERNAME&theme=onedark&no-frame=true&row=1)](https://github.com/ryo-ma/github-profile-trophy)
```

### 👀 Preview

<div align="center">

[![trophy](https://github-profile-trophy.vercel.app/?username=drnecrotix&theme=onedark&no-frame=true&row=1)](https://github.com/ryo-ma/github-profile-trophy)

</div>

### Useful parameters

```text
username=USERNAME
theme=onedark
no-frame=true
row=1
column=6
```

> [!NOTE]
> This is an external Vercel-hosted service. If it becomes unavailable, GitHub may show only the image alt text.

Project: [ryo-ma/github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy)

---

# 📈 Activity Graph

This graph visualizes recent GitHub contribution activity.

### Code

```md
[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=USERNAME&theme=github-dark&hide_border=true)](https://github.com/Ashutosh00710/github-readme-activity-graph)
```

### 👀 Preview

<div align="center">

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=drnecrotix&theme=github-dark&hide_border=true)](https://github.com/Ashutosh00710/github-readme-activity-graph)

</div>

The project currently documents `github-readme-activity-graph.vercel.app` as its canonical deployment.

Project: [Ashutosh00710/github-readme-activity-graph](https://github.com/Ashutosh00710/github-readme-activity-graph)

---

# 💬 Dynamic Quote

A rotating programming quote can add personality without requiring user authentication.

### Code

```md
[![Readme Quotes](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=github_dark)](https://github.com/PiyushSuthar/github-readme-quotes)
```

### 👀 Preview

<div align="center">

[![Readme Quotes](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=github_dark)](https://github.com/PiyushSuthar/github-readme-quotes)

</div>

### Custom quote

```md
[![Readme Quotes](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=github_dark&quote=Build%20something%20useful&author=Your%20Name)](https://github.com/PiyushSuthar/github-readme-quotes)
```

Project: [PiyushSuthar/github-readme-quotes](https://github.com/PiyushSuthar/github-readme-quotes)

---

# 🐍 Contribution Snake

The snake animation is generated from a GitHub contribution graph using **GitHub Actions**. This is more reliable than requesting a new dynamic image on every profile visit because the generated SVG is stored in your repository.

## Workflow example

Create:

```text
.github/workflows/snake.yml
```

Then add:

```yaml
name: Generate contribution snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest

    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark

      - name: Publish generated files
        uses: crazy-max/ghaction-github-pages@v4
        with:
          build_dir: dist
          target_branch: output
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

Then embed the generated image:

```html
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/USERNAME/USERNAME/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/USERNAME/USERNAME/output/github-snake.svg" />
  <img alt="GitHub contribution snake" src="https://raw.githubusercontent.com/USERNAME/USERNAME/output/github-snake.svg" />
</picture>
```

Project: [Platane/snk](https://github.com/Platane/snk)

---

# 📌 Pinned Repository Cards

GitHub Readme Stats supports repository cards, but its shared public Vercel deployment is best-effort. For a stable profile, use **GitHub Actions-generated static cards** or your own instance.

### Self-hosted example

```md
[![Project Card](https://YOUR-STATS-DOMAIN.example/api/pin/?username=USERNAME&repo=REPOSITORY&theme=github_dark)](https://github.com/USERNAME/REPOSITORY)
```

### Two cards side by side

```html
<a href="https://github.com/USERNAME/PROJECT_ONE">
  <img height="120" src="https://YOUR-STATS-DOMAIN.example/api/pin/?username=USERNAME&repo=PROJECT_ONE&theme=github_dark" />
</a>
<a href="https://github.com/USERNAME/PROJECT_TWO">
  <img height="120" src="https://YOUR-STATS-DOMAIN.example/api/pin/?username=USERNAME&repo=PROJECT_TWO&theme=github_dark" />
</a>
```

Project: [anuraghazra/github-readme-stats](https://github.com/anuraghazra/github-readme-stats)

> [!IMPORTANT]
> For this repository, the shared public `github-readme-stats.vercel.app` endpoint is deliberately **not** used as the default because it can fail under rate limits and traffic spikes.

---

# ⏱️ WakaTime Coding Activity

WakaTime is useful when you want to show actual coding-time data instead of only GitHub commits.

GitHub Readme Stats can generate a WakaTime card, but for reliability the recommended setup here is again a self-hosted or GitHub Actions-generated card.

### Example

```md
[![WakaTime](https://YOUR-STATS-DOMAIN.example/api/wakatime?username=WAKATIME_USERNAME&theme=github_dark)](https://wakatime.com/)
```

For this to work, the relevant WakaTime profile statistics need to be public.

### Simpler badge alternative

```md
[![wakatime](https://wakatime.com/badge/user/YOUR_WAKATIME_ID.svg)](https://wakatime.com/@YOUR_WAKATIME_ID)
```

> [!NOTE]
> Replace `YOUR_WAKATIME_ID` with the value provided by your own WakaTime badge page. Do not copy another user's ID.

---

# 🎵 Spotify / Now Playing

Spotify widgets normally require you to authorize your Spotify account with the widget provider first.

A popular open-source option is **spotify-github-profile**.

## Setup

1. Open the project's deployment/setup page.
2. Connect your Spotify account.
3. Copy the generated image URL.
4. Paste the generated code into your README.

Typical generated structure:

```md
[![Spotify](YOUR_GENERATED_SPOTIFY_WIDGET_URL)](https://open.spotify.com/)
```

Do **not** use somebody else's generated identifier because the card would display their listening activity instead of yours.

Project: [kittinan/spotify-github-profile](https://github.com/kittinan/spotify-github-profile)

---

# 🟣 Discord Presence

Discord presence cards require your **Discord user ID** and usually a third-party presence service or a self-hosted integration.

A safe template is:

```md
[![Discord Presence](YOUR_DISCORD_PRESENCE_SVG_URL)](https://discord.com/users/YOUR_DISCORD_USER_ID)
```

Before publishing:

1. verify which service generates the SVG;
2. confirm that you are comfortable exposing your Discord user ID;
3. replace `YOUR_DISCORD_USER_ID`;
4. verify the image does not expose information you do not want public.

> [!WARNING]
> Presence widgets may expose online status, current activities or other Discord information. Only enable them if you intentionally want that information public.

---

# 🌍 Visitor Tracking

A normal profile view badge is less invasive than a geographic visitor map:

```md
![Profile Views](https://komarev.com/ghpvc/?username=USERNAME&label=Profile%20Views&style=flat)
```

For a visitor **map**, use a service only after reviewing its privacy policy and data retention behavior. A map can involve processing visitor IP addresses or geographic information, so this template does not recommend a tracking-map provider by default.

> [!TIP]
> If your goal is simply to know whether people are viewing your repositories, GitHub's own repository **Insights → Traffic** page provides visitor information to users with push access without adding a public tracker to the README.

---

# 🛡️ Reliability Guide

| Widget | Setup | Reliability | Notes |
| --- | --- | --- | --- |
| **Typing SVG** | Easy | Good | External SVG service |
| **Streak Stats** | Easy | Good | External service |
| **Profile Views** | Easy | Good | External counter |
| **GitHub Trophies** | Easy | Medium | External Vercel service |
| **Activity Graph** | Easy | Medium–Good | Canonical external deployment |
| **Dynamic Quote** | Easy | Medium | External Vercel service |
| **Contribution Snake** | Medium | **High** | Generated with GitHub Actions |
| **Pinned Cards** | Medium | **High when self-hosted/static** | Avoid shared public stats endpoint |
| **WakaTime** | Medium | High with own setup | Requires WakaTime account |
| **Spotify** | Medium | Medium | Requires authorization |
| **Discord Presence** | Medium | Medium | Privacy considerations |
| **Visitor Map** | Varies | Varies | Privacy considerations |

---

## Recommended combination

For a profile that looks dynamic without becoming fragile:

```text
Typing Header
↓
Tech Stack
↓
Featured Projects
↓
Activity Graph
↓
Contribution Snake
↓
GitHub Streak
↓
Profile Views
```

Use Spotify, Discord presence, WakaTime, trophies and dynamic quotes only when they add useful information to your specific profile.

---

<div align="center">

### Keep your README useful first, dynamic second.

[![Back to README](https://img.shields.io/badge/Back_to-README-181717?style=for-the-badge&logo=github)](README.md)
[![Live Preview](https://img.shields.io/badge/View-Live_Preview-0969da?style=for-the-badge)](LIVE_PREVIEW.md)

</div>
