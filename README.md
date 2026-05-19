# shadowfox.se

Portfolio website for the ShadowFox security tools project. Live at **[shadowfox.se](https://shadowfox.se)**.

## About

Static site built with plain HTML and CSS — no frameworks or build steps. Hosted via GitHub Pages.

Presents the open-source security tools built under the ShadowFox brand, each with a dedicated technical writeup covering project structure, core functionality, and engineering challenges.

## Structure

| Path | Content |
|------|---------|
| `index.html` | Landing page — tool overview, writeups, lab notes, footer |
| `reports/` | Technical writeups and lab notes (one HTML file per report) |
| `assets/` | Images and logos |

## Run locally

```bash
git clone https://github.com/elin-olsson/elin-olsson.github.io.git
cd elin-olsson.github.io
python3 -m http.server 8080
```

Open `http://localhost:8080` in a browser.

## Tools

| Tool | Repo | Status |
|------|------|--------|
| ssh-tls-auditor | [github.com/elin-olsson/ssh-tls-auditor](https://github.com/elin-olsson/ssh-tls-auditor) | Live |
| chain-watch | [github.com/elin-olsson/chain-watch](https://github.com/elin-olsson/chain-watch) | Live |
| fox-trace | [github.com/elin-olsson/fox-trace](https://github.com/elin-olsson/fox-trace) | Live |
| ghost-trail | [github.com/elin-olsson/ghost-trail](https://github.com/elin-olsson/ghost-trail) | Live |
| ShadowFox VDI | [github.com/elin-olsson/ShadowFox-VDI](https://github.com/elin-olsson/ShadowFox-VDI) | In progress |

---

<sub>© 2026 shadowfox.se</sub>
