# shadowfox.se

Portfolio website for the ShadowFox security tools project. Live at **[shadowfox.se](https://shadowfox.se)**.

## About

Static site built with plain HTML and CSS — no frameworks or build steps. Hosted via GitHub Pages.

Presents the open-source security tools built under the ShadowFox brand, each with a dedicated technical writeup covering project structure, core functionality, and engineering challenges.

## Structure

| File | Content |
|------|---------|
| `index.html` | Landing page — tool overview, lab notes, footer |
| `chain-watch-report.html` | Technical writeup for chain-watch |
| `fox-trace-report.html` | Technical writeup for fox-trace |
| `ghost-trail-report.html` | Technical writeup for ghost-trail |
| `ssh-tls-auditor-report.html` | Technical writeup for ssh-tls-auditor |
| `rpi-setup-report.html` | Lab note — Raspberry Pi subnet router setup |
| `router-incident-report.html` | Lab note — Suricata IPS incident |

## Run locally

```bash
git clone https://github.com/elin-olsson/elin-olsson.github.io.git
cd elin-olsson.github.io
python3 -m http.server 8080
```

Open `http://localhost:8080` in a browser.

## Tools

| Tool | Repo |
|------|------|
| ssh-tls-auditor | [github.com/elin-olsson/ssh-tls-auditor](https://github.com/elin-olsson/ssh-tls-auditor) |
| chain-watch | [github.com/elin-olsson/chain-watch](https://github.com/elin-olsson/chain-watch) |
| fox-trace | [github.com/elin-olsson/fox-trace](https://github.com/elin-olsson/fox-trace) |
| ghost-trail | [github.com/elin-olsson/ghost-trail](https://github.com/elin-olsson/ghost-trail) |

---

<sub>© 2026 shadowfox.se</sub>
