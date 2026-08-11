# 👾 Dr. Necrotix Profile README

A reusable GitHub Profile README template created by **Dr.Necrotix [NIKO]**.

Use it as a starting point for building a clean developer profile with social links, technology badges, featured projects, GitHub statistics and customizable content sections.

> This repository is a **GitHub Profile README template**. It is not a WordPress plugin and does not provide WordPress shortcodes.

---

## ✨ Features

- Clean GitHub profile layout
- Social and website badges
- About Me section
- Technology / tools section
- Featured projects
- GitHub statistics cards
- GitHub streak statistics
- Profile view counter
- Easy Markdown customization
- Ready to use as a GitHub repository template

---

## 🚀 Quick Start

### Option 1 — Use this repository as a template

1. Click **Use this template** at the top of this repository.
2. Choose **Create a new repository**.
3. For a GitHub profile README, name the new repository exactly the same as your GitHub username.

Example:

```text
GitHub username: exampleuser
Repository name: exampleuser
```

4. Make the repository **Public**.
5. Open `README.md`.
6. Replace the example information with your own details.
7. Commit the changes.

GitHub will automatically display that README on your profile page.

### Option 2 — Copy only the parts you need

You do not need to use the entire template. Open `README.md`, copy the desired section and paste it into your own profile README.

---

# 🧩 Reusable README Snippets

The blocks below work like reusable components. Copy the snippet you want and replace the example values.

## Profile heading

```md
<div align="center">

# 👾 Your Name

### Developer • Designer • Creator

</div>
```

Change:

- `Your Name`
- the subtitle
- the emoji if desired

---

## Social badges

```md
[![GitHub](https://img.shields.io/badge/GitHub-USERNAME-181717?style=for-the-badge&logo=github)](https://github.com/USERNAME)
[![Website](https://img.shields.io/badge/Website-example.com-0A66C2?style=for-the-badge)](https://example.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/USERNAME)
```

Replace every `USERNAME` and example URL with your own information.

### Badge structure

A Shields.io badge normally follows this format:

```text
https://img.shields.io/badge/LABEL-MESSAGE-COLOR
```

Example:

```md
![My Project](https://img.shields.io/badge/My_Project-Active-success)
```

---

## About Me section

```md
## 🧬 About Me

I'm **Your Name**, a developer and digital creator focused on building useful projects and experimenting with new technologies.

- 🔭 Working on **Project Name**
- 🧩 Building **plugins and tools**
- 🤖 Interested in **automation and AI**
- 🌐 Working with **web technologies**
```

Edit or remove any lines you do not need.

---

## Technology icons

This template uses **Skill Icons**.

```html
<div align="center">

<img src="https://skillicons.dev/icons?i=html,css,js,ts,react,nodejs,php,mysql,git,github&perline=5" alt="Tech stack" />

</div>
```

### Adding or removing technologies

Edit the value after:

```text
i=
```

Example:

```text
i=html,css,js,react,php
```

The `perline` parameter controls how many icons appear on each row:

```text
&perline=5
```

Example with 8 icons per row:

```text
&perline=8
```

---

## Technology text list

```md
`JavaScript` · `TypeScript` · `React` · `PHP` · `WordPress` · `MySQL`
```

Simply replace the technology names.

---

## Featured project

```md
### 🚀 [Project Name](https://github.com/USERNAME/REPOSITORY)
Short description explaining what the project does.

**Stack:** JavaScript · React · Node.js
```

Duplicate the block for additional projects.

---

# 📊 GitHub Statistics

## GitHub stats card

```html
<img src="https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true&hide_border=true&theme=github_dark" alt="GitHub stats" />
```

Replace:

```text
USERNAME
```

with your GitHub username.

### Common parameters

```text
show_icons=true
hide_border=true
theme=github_dark
```

Parameters are joined using `&`.

Example:

```text
?username=USERNAME&show_icons=true&hide_border=true&theme=github_dark
```

---

## Most used languages

```html
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=USERNAME&layout=compact&hide_border=true&theme=github_dark" alt="Most used languages" />
```

Useful parameter:

```text
layout=compact
```

This displays languages in a smaller compact card.

---

## GitHub streak

```html
<img src="https://github-readme-streak-stats.herokuapp.com/?user=USERNAME&theme=github-dark-blue&hide_border=true" alt="GitHub streak" />
```

Replace `USERNAME` with your GitHub username.

---

## Profile views

```html
<img src="https://komarev.com/ghpvc/?username=USERNAME&label=Profile%20Views&style=flat" alt="Profile views" />
```

Available values you may customize include:

```text
username=USERNAME
label=Profile%20Views
style=flat
```

---

# 🎨 Layout Helpers

## Center content

```html
<div align="center">

Your content here

</div>
```

Useful for:

- headings
- badges
- statistics
- images
- icons

---

## Add a separator

```md
---
```

This creates a horizontal divider.

---

## Add line spacing

```html
<br />
```

Use it sparingly. Too many `<br />` tags can create large empty spaces in a profile README.

---

## Add an image

```html
<img src="IMAGE_URL" alt="Description" />
```

With a custom width:

```html
<img width="500" src="IMAGE_URL" alt="Description" />
```

---

## Add a clickable image

```html
<a href="https://example.com">
  <img src="IMAGE_URL" alt="Example" />
</a>
```

This is useful when technology icons, project logos or banners should open another website when clicked.

---

# 🔗 Open Links in a New Tab

GitHub sanitizes rendered README HTML and does **not reliably support forcing links to open in a new browser tab** with `target="_blank"`.

For maximum GitHub compatibility, use standard links:

```html
<a href="https://example.com">Example</a>
```

or Markdown:

```md
[Example](https://example.com)
```

The visitor's browser/GitHub interface determines how the link is opened.

---

# 🛠️ Create Your Own Profile

A recommended profile structure is:

```text
Header
↓
Social links
↓
About Me
↓
Tech & Tools
↓
Featured Projects
↓
GitHub Stats
↓
Interests
↓
Contact / Social links
```

Keep the most important information near the top because visitors usually scan a profile before reading it in detail.

---

# ⚠️ Common Problems

## The README does not appear on my GitHub profile

Make sure:

1. The repository name is exactly your GitHub username.
2. The repository is public.
3. The file is named `README.md`.
4. `README.md` exists in the repository's default branch.

---

## Images are not loading

Check that:

- the image URL is public;
- the URL uses HTTPS;
- the external service is online;
- the URL has not expired.

---

## GitHub stats are not updating immediately

External statistics services may cache results. Changes to your profile or repositories may therefore take some time to appear in generated statistics cards.

---

## My README has large empty spaces

Avoid excessive use of:

```html
<br />
```

Also verify that HTML containers such as `<div>` and `<p>` are correctly closed.

---

# 👨‍💻 Example Author Setup

The original template is maintained by:

**Dr.Necrotix [NIKO]**

- GitHub: [@drnecrotix](https://github.com/drnecrotix)
- Website: [BG-GAMER](https://bg-gamer.com/)
- Discord: [BG-GAMER Community](https://discord.bg-gamer.com/)
- LinkedIn: [Dr. Necrotix](https://www.linkedin.com/in/necrotix/)
- Instagram: [@dr.necrotix](https://instagram.com/dr.necrotix)

---

## 📄 License

This repository is released under **The Unlicense**.

You may copy, modify and reuse the template for your own GitHub profile.

---

<div align="center">

### 💀 Build. Break. Learn. Improve. Repeat.

Made by **Dr.Necrotix [NIKO]**

</div>
