<div align="center">

# 👾 GitHub Profile README Template

### Build a polished GitHub profile without starting from scratch.

[![Use this template](https://img.shields.io/badge/Use_this_template-2ea44f?style=for-the-badge&logo=github&logoColor=white)](https://github.com/new?template_name=profile-readme&template_owner=drnecrotix)
[![Live Preview](https://img.shields.io/badge/👀_Live-Preview-0969da?style=for-the-badge)](LIVE_PREVIEW.md)
[![GitHub](https://img.shields.io/badge/Author-Dr.Necrotix-181717?style=for-the-badge&logo=github)](https://github.com/drnecrotix)
[![License](https://img.shields.io/badge/License-Unlicense-blue?style=for-the-badge)](LICENSE)

A reusable collection of **GitHub Profile README components** with copy-and-paste examples, customization notes and rendered previews.

</div>

> [!NOTE]
> This repository is a **GitHub Profile README template**, not a WordPress plugin. The examples are reusable Markdown and GitHub-compatible HTML snippets.

---

## 📚 Contents

- [Live Preview](LIVE_PREVIEW.md)
- [Quick Start](#-quick-start)
- [Profile Header](#-profile-header)
- [Social Badges](#-social-badges)
- [About Me](#-about-me)
- [Tech Stack](#-tech-stack)
- [Featured Projects](#-featured-projects)
- [GitHub Activity](#-github-activity)
- [Profile Views](#-profile-views)
- [Images & Layout](#-images--layout)
- [Complete Profile Example](#-complete-profile-example)
- [Troubleshooting](#-troubleshooting)

---

# 🚀 Quick Start

## 1. Create your profile repository

Click **Use this template** → **Create a new repository**.

For GitHub to display the README on your profile, the repository name must be exactly the same as your GitHub username.

```text
GitHub username: octocat
Repository name: octocat
```

The repository should be **Public** and contain a `README.md` file in its default branch.

## 2. Replace the example values

Look for values such as:

```text
YOUR_NAME
USERNAME
YOUR_WEBSITE
PROJECT_NAME
REPOSITORY
```

Replace them with your own details.

## 3. Preview your changes

Use GitHub's **Preview** tab while editing `README.md` to check spacing, badges, links and images before committing.

> [!TIP]
> Start simple. You can always add more components later.

---

# 👤 Profile Header

### Code

```html
<div align="center">

# 👋 Hi, I'm Alex

### Developer • Designer • Open-source enthusiast

I build useful tools and enjoy learning new technologies.

</div>
```

### 👀 Preview

<div align="center">

# 👋 Hi, I'm Alex

### Developer • Designer • Open-source enthusiast

I build useful tools and enjoy learning new technologies.

</div>

---

# 🔗 Social Badges

Badges are a compact way to link your GitHub profile, website, portfolio and social accounts.

### Code

```md
[![GitHub](https://img.shields.io/badge/GitHub-USERNAME-181717?style=for-the-badge&logo=github)](https://github.com/USERNAME)
[![Website](https://img.shields.io/badge/Website-Portfolio-21759B?style=for-the-badge&logo=googlechrome&logoColor=white)](https://example.com/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/USERNAME)
```

### 👀 Preview

[![GitHub](https://img.shields.io/badge/GitHub-drnecrotix-181717?style=for-the-badge&logo=github)](https://github.com/drnecrotix)
[![Website](https://img.shields.io/badge/Website-BG--GAMER-21759B?style=for-the-badge&logo=wordpress&logoColor=white)](https://bg-gamer.com/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/necrotix/)

## Badge structure

```text
https://img.shields.io/badge/LABEL-MESSAGE-COLOR?style=STYLE&logo=LOGO
```

| Part | Purpose | Example |
| --- | --- | --- |
| `LABEL` | Left part of the badge | `GitHub` |
| `MESSAGE` | Main badge text | `drnecrotix` |
| `COLOR` | Badge color | `181717` |
| `style` | Badge style | `for-the-badge` |
| `logo` | Optional logo | `github` |
| `logoColor` | Optional logo color | `white` |

---

# 🧬 About Me

Keep this section short and focused on what you build, learn and contribute to.

### Code

```md
## 🧬 About Me

I'm **Alex**, a developer who enjoys building practical web applications and open-source tools.

- 🔭 Currently working on **Project Nova**
- 🌱 Learning **TypeScript and Cloudflare Workers**
- 🧩 Building **plugins, APIs and integrations**
- 🤖 Interested in **automation and AI-assisted development**
- 💬 Ask me about **JavaScript, PHP and APIs**
```

### 👀 Preview

## 🧬 About Me

I'm **Alex**, a developer who enjoys building practical web applications and open-source tools.

- 🔭 Currently working on **Project Nova**
- 🌱 Learning **TypeScript and Cloudflare Workers**
- 🧩 Building **plugins, APIs and integrations**
- 🤖 Interested in **automation and AI-assisted development**
- 💬 Ask me about **JavaScript, PHP and APIs**

---

# 🛠️ Tech Stack

## Skill Icons

### Code

```html
<div align="center">
  <img src="https://skillicons.dev/icons?i=html,css,js,ts,react,nodejs,php,mysql,git,github&perline=5" alt="Tech stack" />
</div>
```

### 👀 Preview

<div align="center">
  <img src="https://skillicons.dev/icons?i=html,css,js,ts,react,nodejs,php,mysql,git,github&perline=5" alt="Tech stack" />
</div>

Edit the values after `i=` to choose icons:

```text
i=html,css,js,react,php
```

Control the number of icons per row with:

```text
&perline=5
```

## Text-only stack

### Code

```md
`JavaScript` · `TypeScript` · `React` · `PHP` · `WordPress` · `MySQL`
```

### 👀 Preview

`JavaScript` · `TypeScript` · `React` · `PHP` · `WordPress` · `MySQL`

---

# 🚀 Featured Projects

Show a few projects that best represent your work instead of listing every repository.

### Code

```md
### 🚀 [Project Nova](https://github.com/USERNAME/project-nova)

A lightweight dashboard for managing community services and integrations.

**Highlights:** API integrations · Responsive dashboard · Automation

**Stack:** TypeScript · React · Node.js
```

### 👀 Preview

### 🚀 [Project Nova](https://github.com/drnecrotix/profile-readme)

A lightweight dashboard for managing community services and integrations.

**Highlights:** API integrations · Responsive dashboard · Automation

**Stack:** TypeScript · React · Node.js

---

# 📊 GitHub Activity

This template intentionally avoids the public `github-readme-stats.vercel.app` endpoint in its default examples because public third-party statistics endpoints can be rate-limited or temporarily unavailable.

The default setup uses components that currently render more reliably while still giving your profile an activity-focused section.

## GitHub Streak

### Code

```html
<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=USERNAME&theme=github-dark-blue&hide_border=true" alt="GitHub streak" />
</div>
```

### 👀 Live Preview

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=drnecrotix&theme=github-dark-blue&hide_border=true" alt="GitHub streak" />
</div>

Replace `USERNAME` with your GitHub username.

## Optional: GitHub Stats & Top Languages

If you want the traditional GitHub Stats and Top Languages cards, the safer approach is to use **your own deployment** of GitHub Readme Stats or another endpoint you control.

### Self-hosted Stats example

```html
<img src="https://YOUR-STATS-DOMAIN.example/api?username=USERNAME&show_icons=true&theme=github_dark" alt="GitHub stats" />
```

### Self-hosted Top Languages example

```html
<img src="https://YOUR-STATS-DOMAIN.example/api/top-langs/?username=USERNAME&layout=compact&theme=github_dark" alt="Most used languages" />
```

> [!IMPORTANT]
> Do not blindly copy a public statistics endpoint into a production profile. If the provider is rate-limited or unavailable, GitHub will display only the image's `alt` text.

---

# 👁️ Profile Views

### Code

```html
<img src="https://komarev.com/ghpvc/?username=USERNAME&label=Profile%20Views&style=flat" alt="Profile views" />
```

### 👀 Live Preview

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=drnecrotix&label=Profile%20Views&style=flat" alt="Profile views" />
</div>

You can change the label:

```text
label=Profile%20Views
```

`%20` represents a space inside a URL.

---

# 🎨 Images & Layout

## Center content

```html
<div align="center">

Your content here

</div>
```

### Preview

<div align="center">

**This content is centered.**

</div>

## Add an image

```html
<img src="IMAGE_URL" alt="Useful image description" />
```

With a custom width:

```html
<img width="500" src="IMAGE_URL" alt="Useful image description" />
```

## Clickable image

### Code

```html
<a href="https://github.com/">
  <img src="https://img.shields.io/badge/Visit-GitHub-181717?style=for-the-badge&logo=github" alt="Visit GitHub" />
</a>
```

### 👀 Preview

<a href="https://github.com/">
  <img src="https://img.shields.io/badge/Visit-GitHub-181717?style=for-the-badge&logo=github" alt="Visit GitHub" />
</a>

## Separator

```md
---
```

## Manual line break

```html
<br />
```

Use `<br />` sparingly. Too many manual breaks can create large empty spaces.

---

# 🔗 Opening Links in a New Tab

GitHub sanitizes README HTML and does not provide a dependable way to force a README link to open in a new tab.

Use normal Markdown:

```md
[Example](https://example.com)
```

or HTML:

```html
<a href="https://example.com">Example</a>
```

The visitor can use their browser's normal new-tab controls.

---

# 🧱 Complete Profile Example

Copy the example below and replace the placeholder values.

```md
<div align="center">

# 👋 Hi, I'm Alex

### Full-stack Developer • Open-source Enthusiast

[![GitHub](https://img.shields.io/badge/GitHub-USERNAME-181717?style=for-the-badge&logo=github)](https://github.com/USERNAME)
[![Website](https://img.shields.io/badge/Website-Portfolio-0A66C2?style=for-the-badge)](https://example.com)

</div>

## 🧬 About Me

I build practical web applications, integrations and open-source tools.

- 🔭 Working on **Project Nova**
- 🌱 Learning **new web technologies**
- 🤖 Interested in **automation and AI**

## 🛠️ Tech Stack

<div align="center">
  <img src="https://skillicons.dev/icons?i=html,css,js,ts,react,nodejs,php,mysql,git,github&perline=5" alt="Tech stack" />
</div>

## 🚀 Featured Project

### [Project Nova](https://github.com/USERNAME/PROJECT)
A short description of your project and why it is useful.

**Stack:** TypeScript · React · Node.js

## 📊 GitHub Activity

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=USERNAME&theme=github-dark-blue&hide_border=true" alt="GitHub streak" />
  <br />
  <img src="https://komarev.com/ghpvc/?username=USERNAME&label=Profile%20Views&style=flat" alt="Profile views" />
</div>
```

## 👀 Example Result

<div align="center">

# 👋 Hi, I'm Dr. Necrotix

### Developer • WordPress Builder • Digital Creator

[![GitHub](https://img.shields.io/badge/GitHub-drnecrotix-181717?style=for-the-badge&logo=github)](https://github.com/drnecrotix)
[![Website](https://img.shields.io/badge/Website-BG--GAMER-21759B?style=for-the-badge&logo=wordpress&logoColor=white)](https://bg-gamer.com/)

</div>

## 🧬 About Me

I build practical web tools, WordPress extensions, integrations and community-focused projects.

- 🔭 Building projects around **BG-GAMER**
- 🧩 Creating **plugins and integrations**
- 🤖 Interested in **automation, APIs and AI-assisted development**

## 🛠️ Tech Stack

<div align="center">
  <img src="https://skillicons.dev/icons?i=html,css,js,ts,react,nodejs,php,mysql,git,github&perline=5" alt="Tech stack" />
</div>

## 📊 GitHub Activity

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=drnecrotix&theme=github-dark-blue&hide_border=true" alt="GitHub streak" />
  <br />
  <img src="https://komarev.com/ghpvc/?username=drnecrotix&label=Profile%20Views&style=flat" alt="Profile views" />
</div>

---

# ⚠️ Troubleshooting

<details>
<summary><strong>My README does not appear on my profile</strong></summary>

Make sure:

1. the repository name exactly matches your GitHub username;
2. the repository is public;
3. the file is named `README.md`;
4. `README.md` exists in the default branch.

</details>

<details>
<summary><strong>An image or badge is not loading</strong></summary>

Check that the URL is public, uses HTTPS and opens correctly on its own. External image providers may also experience outages or rate limits.

</details>

<details>
<summary><strong>I only see alt text instead of a statistics card</strong></summary>

The external image endpoint is not returning a usable image. Replace it with a working endpoint or use your own deployment of the statistics service.

</details>

<details>
<summary><strong>My README has large empty spaces</strong></summary>

Remove unnecessary `<br />` elements and verify that HTML containers such as `<div>` are correctly closed.

</details>

<details>
<summary><strong>My link does not open in a new tab</strong></summary>

This is expected. GitHub does not provide README authors with a reliable method for forcing links to open in a new tab.

</details>

---

# 👀 Live Preview Gallery

Want to compare complete styles before choosing one?

[![Open Live Preview](https://img.shields.io/badge/👀_Open-Live_Preview-0969da?style=for-the-badge&logo=github)](LIVE_PREVIEW.md)

The gallery includes:

`Minimal` · `Developer` · `Creative` · `Gaming` · `Advanced`

---

# 👨‍💻 Author

<div align="center">

### Dr.Necrotix [NIKO]

[![GitHub](https://img.shields.io/badge/GitHub-drnecrotix-181717?style=flat-square&logo=github)](https://github.com/drnecrotix)
[![Website](https://img.shields.io/badge/BG--GAMER-Website-21759B?style=flat-square&logo=wordpress&logoColor=white)](https://bg-gamer.com/)
[![Discord](https://img.shields.io/badge/BG--GAMER-Discord-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.bg-gamer.com/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Dr.Necrotix-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/necrotix/)
[![Instagram](https://img.shields.io/badge/Instagram-@dr.necrotix-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://instagram.com/dr.necrotix)

</div>

---

## 📄 License

Released under **The Unlicense**. You may copy, modify and reuse this template for your own GitHub profile.

If this template helped you, consider giving the repository a ⭐.

---

<div align="center">

### 💀 Build. Break. Learn. Improve. Repeat.

Made by **Dr.Necrotix [NIKO]**

</div>
