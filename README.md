<p align="center">
  <img width="160px" src="assets/logo.png">
</p>

<h2 align="center"><b>LinkHongest</b></h2>

<h4 align="center">
A lightweight, static multi-link hub<br>
built for clarity, control, and zero backend complexity.
</h4>

---

<p align="center">
  <a href="#overview">Overview</a> •
  <a href="#features">Features</a> •
  <a href="#structure">Project Structure</a> •
  <a href="#routing">Routing Logic</a> •
  <a href="#tech">Tech Stack</a> •
  <a href="#setup">Setup</a> •
  <a href="#deployment">Deployment</a> •
  <a href="#license">License</a>
</p>

---

## Overview

**LinkHongest** is a fully static website designed to route a single domain to multiple destinations.

It supports:
- Root-level redirects (e.g. Discord)
- Multiple subpaths serving independent pages
- Zero backend, zero database, zero runtime dependencies

Everything is handled via static files and server-side routing.

---

## Features

- 📌 Multiple destinations under one domain
- 🔀 Root-level redirect support
- 📁 Folder-based URL routing
- 🎥 Video & audio support
- 🎨 Custom fonts and assets
- 📱 Responsive layouts
- ⚡ CDN-powered performance
- 🔒 No cookies, no analytics, no tracking

---

## Project Structure

Folder-based routing maps directories directly to URLs:

```

/
├─ _redirects          → Cloudflare Pages routing rules
│
├─ assets/             → Shared icons and images
│  ├─ 1.png
│  ├─ 2.png
│  ├─ 3.png
│  ├─ 4.png
│  ├─ 5.png
│  └─ logo.png
├─ kkaan.gull/
│  ├─ index.html       → /kkaan.gull
│  ├─ video.mp4
│  ├─ ses.mp3
│  ├─ profil.jpg
│  └─ herseyfont.otf
│
└─ guns/
│  ├─ index.html       → /guns
│  ├─ video.mp4
│  ├─ ses.mp3
│  ├─ profil.png
│  └─ herseyfont.otf

```

Each folder maps directly to its URL path.

---

## Routing Logic

Routing is handled **server-side** using Cloudflare Pages.

Example `_redirects` rule:

```

/ [https://discord.gg/2xSPvuyKWg](https://discord.gg/2xSPvuyKWg) 302

```

This means:
- `/` → Discord
- `/kkaan.gull` → `kkaan.gull/index.html`
- `/guns` → `guns/index.html`

No client-side JavaScript redirects are required.

---

## Tech Stack

Built with **pure web technologies** only:

- HTML5
- CSS3
- Vanilla JavaScript
- Static media assets (MP4, MP3, PNG, OTF)

No frameworks  
No libraries  
No build tools  

---

## Setup

1. Clone or download the repository
2. Keep the folder structure unchanged
3. Edit content inside:
   - `index.html`
   - `kkaan.gull/index.html`
   - `guns/index.html`
4. Replace assets as needed (images, video, audio)

No installation or configuration required.

---

## Deployment

LinkHongest can be deployed on any static hosting provider.

Recommended:
- **Cloudflare Pages**

Also compatible with:
- GitHub Pages
- Netlify
- Any static web host

Requirements:
- Static file hosting only

You do **NOT** need:
- PHP
- SQL / MySQL
- Node.js
- Docker

---

## License

This project is intended for **personal and internal use**.

You are free to:
- Modify the source
- Change routing and content
- Deploy under your own domain

No warranty is provided.

---

<p align="center">
  LinkHongest • Part of the Hongest ecosystem
</p>
