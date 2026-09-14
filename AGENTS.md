# Agent notes — yhkcyber.github.io

Personal link page for Yegor H. Kryvenka (GitHub Pages, served from `main`).

## Conventions

- Single file: `index.html` holds all HTML, CSS and JS. No build step, no dependencies beyond Google Fonts (JetBrains Mono).
- Keep it simple and fast: dark terminal aesthetic, one accent color (`--acc: #6ee4a5`), no images, no frameworks.
- Content lives in two places in `index.html`: the static `whoami` / `help` blocks in `<body>`, and the `PROJECTS`, `WRITEUPS`, `COMPETITIONS`, `LINKS` arrays at the top of the `<script>`. Edit data there rather than adding markup.
- LinkedIn (`https://www.linkedin.com/in/yegorkryvenka`) is the primary call to action; everything else is secondary.
- Facts on the page come from Yegor's resume — don't invent roles, dates or numbers. Unknown facts go in as a visibly marked `[TODO: …]` line, which renders red, so they get noticed before shipping.
- Preview locally with `python3 -m http.server 8000`. Deploy is just `git push` to `main`.

## Handoff Notes

- 2026-09-14: Rebuilt the site from the old video-background link page into the terminal design (concept "B" from the design canvas). Working terminal: clickable command chips, typed commands, Tab completion, ↑/↓ history, Ctrl+L / Ctrl+C.
- Open item: the `raptorhacks` project entry has a red `[TODO]` line — Yegor's role in RaptorHacks 2026 is not stated on the resume or raptorhacks.com. Fill it in before or right after publishing.
- Open item: `WRITEUPS` is empty by design; the `writeups` command shows a "coming soon" message until entries are added.
- The wins counter counts podium finishes (1st PICMC/MAGIC CTF 18, 2nd Lockheed Martin CyberQuest, 3rd VelocityX) = 3. Change `data-count` and the `COMPETITIONS` array together if that rule changes.
- LinkedIn profile could not be read from this machine (auth wall); content was taken from the September 2026 resume.
