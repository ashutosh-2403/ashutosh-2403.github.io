<div align="center">

```
   █████╗ ███████╗██╗  ██╗██╗   ██╗████████╗ ██████╗ ███████╗██╗  ██╗
  ██╔══██╗██╔════╝██║  ██║██║   ██║╚══██╔══╝██╔═══██╗██╔════╝██║  ██║
  ███████║███████╗███████║██║   ██║   ██║   ██║   ██║███████╗███████║
  ██╔══██║╚════██║██╔══██║██║   ██║   ██║   ██║   ██║╚════██║██╔══██║
  ██║  ██║███████║██║  ██║╚██████╔╝   ██║   ╚██████╔╝███████║██║  ██║
  ╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝ ╚═════╝    ╚═╝    ╚═════╝ ╚══════╝╚═╝  ╚═╝
```

# ashutosh.portfolio

**A terminal-themed developer portfolio — built with vanilla HTML, CSS, and JavaScript.**

[![Live](https://img.shields.io/badge/live-ashutosh--2403.github.io-00ff88?style=flat-square&logo=github)](https://ashutosh-2403.github.io/)
[![Made with](https://img.shields.io/badge/made%20with-HTML%20%2F%20CSS%20%2F%20JS-f5e642?style=flat-square)](#)
[![License](https://img.shields.io/badge/license-MIT-4db8ff?style=flat-square)](#license)

🔗 **[https://ashutosh-2403.github.io/](https://ashutosh-2403.github.io/)**

</div>

---

## Overview

A fully interactive terminal-style portfolio that runs entirely in the browser — no frameworks, no build tools, no dependencies. Visitors navigate the portfolio by typing commands (or clicking quick-access chips), exploring projects, experience, skills, and contact info just like they would in a real shell.

---

## Features

- **Interactive Terminal UI** — Type commands to explore content; supports Tab autocomplete, ↑↓ command history, and instant output rendering
- **Animated ASCII Banner** — Glowing header rendered in pure CSS with a pulse keyframe animation
- **Particle Network Background** — Canvas-based floating particle mesh with dynamic line connections
- **Custom Cursor** — Smooth lag cursor + dot combo with hover expansion states
- **CRT Scanline Overlay** — Subtle CSS repeating-gradient scanline effect for that authentic terminal feel
- **Live Clock** — Displays real-time `HH:MM:SS` in the title bar
- **Status Bar** — Sticky bottom bar showing command count, last command, and online indicator
- **Autocomplete Dropdown** — Fuzzy prefix-matched suggestions with keyboard navigation
- **Theme Toggle** — Switch between dark (default) and light mode via `theme -light` / `theme -dark`
- **Responsive** — Mobile-friendly layout with cursor and scanline effects gracefully disabled on touch devices

---

## Commands

| Command | Description |
|---|---|
| `about` | Short bio — who I am and what I do |
| `projects` | All projects with tech stack, dates, and GitHub links |
| `skills` | Full tech stack grouped by category |
| `experience` | Internship and work history |
| `education` | PDEU B.Tech details |
| `contact` | Email, phone, GitHub, location |
| `documentation` | Notion docs and notes |
| `help` | Lists all available commands |
| `clear` | Clears the terminal output |
| `theme -light` | Switch to light theme |
| `theme -dark` | Switch back to dark theme |

**Keyboard shortcuts:**
- `Tab` — autocomplete current input
- `↑` / `↓` — cycle through command history
- `Escape` — dismiss autocomplete dropdown
- `Enter` — run command

---

## Tech Stack

This is a **zero-dependency, zero-build** project.

- **HTML5** — semantic structure and canvas element
- **CSS3** — custom properties, keyframe animations, CRT scanline via `repeating-linear-gradient`, sticky bars, responsive layout
- **Vanilla JavaScript** — terminal engine, command dispatcher, autocomplete, Canvas 2D particle system, requestAnimationFrame cursor loop

No React. No Webpack. No npm. Just one `.html` file.

---

## Project Structure

```
portfolio/
└── index.html        # Everything — markup, styles, and scripts in one file
```

---

## Local Development

No setup required. Just clone and open:

```bash
git clone https://github.com/ashutosh-2403/ashutosh-2403.github.io.git
cd ashutosh-2403.github.io
open index.html        # macOS
# or
start index.html       # Windows
# or
xdg-open index.html    # Linux
```

---

## Deployment

Hosted on **GitHub Pages** — any push to `main` automatically deploys to:

```
https://ashutosh-2403.github.io/
```

No CI configuration needed. GitHub Pages serves the root `index.html` directly.

---

## Customization

All content lives inside the `cmds` object in the `<script>` block. To update your own details:

```js
const cmds = {
  about: `...your HTML string...`,
  projects: `...your HTML string...`,
  // etc.
};
```

Colors and theming are controlled via CSS custom properties at the top of the `<style>` block:

```css
:root {
  --bg: #060a06;
  --g1: #00ff88;   /* primary accent */
  --y:  #f5e642;   /* command yellow */
  --b:  #4db8ff;   /* link blue */
  /* ... */
}
```

---

## Screenshots

> _Terminal dark mode (default)_

```
[ashutosh@portfolio] ~ ⎇ main ❯ projects
```

> _Try it live → [https://ashutosh-2403.github.io/](https://ashutosh-2403.github.io/)_

---

## Author

**Ashutosh Mishra**
B.Tech CSE · PDEU '26 · Backend Developer

- GitHub: [@ashutosh-2403](https://github.com/ashutosh-2403)
- Email: ashutoshmishra2403@gmail.com

---

## License

MIT — feel free to fork, adapt, and build your own terminal portfolio. A credit or star is always appreciated. ⭐
