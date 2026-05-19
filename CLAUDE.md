# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Run locally

```bash
python3 -m http.server 8080
```

No build step, no dependencies. Plain HTML/CSS deployed via GitHub Pages to shadowfox.se.

## Architecture

All styling is inline in each HTML file — there is no shared CSS file. Changes to styles must be applied to each file individually.

### index.html

Landing page with three sections: **Security Tools**, **Tool Writeups**, and **Lab Notes**.

**Security Tools** uses `display: flex; flex-wrap: wrap` with `.tool-card` (width 350px desktop, 100% mobile). Tools are grouped under `// comment`-style labels using `.tool-group-label` divs. Current groups:
- `// network auditing` — ssh-tls-auditor
- `// host & forensics` — chain-watch, fox-trace, ghost-trail
- `// infrastructure` — ShadowFox VDI (marked IN PROGRESS with `.coming-soon-badge`)

**Tool Writeups** and **Lab Notes** use `display: flex; flex-wrap: wrap` with `.report-card` (`flex: 1 1 380px`, max-width 430px desktop; `flex: 1 1 100%` on mobile via media query at max-width 768px).

### reports/*.html

Each report file is self-contained with identical CSS structure:
- `.container { max-width: 800px; width: 100%; box-sizing: border-box; padding: 60px 20px; }`
- `table { display: block; overflow-x: auto; }` — required for mobile
- `th, td { word-break: break-word; }` — required for mobile
- `pre { overflow-x: auto; }`

When adding a new report file, copy the CSS block from an existing report (e.g. `ghost-trail-report.html`) — all reports share the same base styles.

## Design system

- Background: `#050a0f`, surface: `#0d141b`, border: `#1a2a3a`
- Accent: `#00d4ff`, muted text: `#8a9baa`, dimmed: `#5a6b7a`
- Headings: `'Courier New'`, body: `'Segoe UI'`
- No emojis, no frameworks, no JavaScript except the D3 timeline embedded in ghost-trail's exported HTML output
