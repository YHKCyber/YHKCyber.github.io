# Agent notes — yhkcyber.github.io

Personal link page for Yegor H. Kryvenka (GitHub Pages, served from `main`).

## Conventions

- Single file: `index.html` holds all HTML, CSS and JS. No build step, no dependencies beyond Google Fonts (JetBrains Mono).
- Keep it simple and fast: dark terminal aesthetic, one accent color (`--acc: #6ee4a5`), no images, no frameworks.
- Content lives in two places in `index.html`: the static `whoami` / `help` blocks in `<body>`, and the `PROJECTS`, `WRITEUPS`, `COMPETITIONS`, `LINKS` arrays at the top of the `<script>`. Edit data there rather than adding markup.
- `/resume` is a redirect page (`resume/index.html`) pointing at the newest PDF in `resume/`. New resume = add the PDF, update the filename in that page.
- LinkedIn (`https://www.linkedin.com/in/yegorkryvenka`) is the primary call to action; everything else is secondary.
- Facts on the page come from Yegor's resume — don't invent roles, dates or numbers. Unknown facts go in as a visibly marked `[TODO: …]` line, which renders red, so they get noticed before shipping.
- Preview locally with `python3 -m http.server 8000`. Deploy is just `git push` to `main`.

## Handoff Notes

- 2026-09-14: Rebuilt the site from the old video-background link page into the terminal design (concept "B" from the design canvas). Working terminal: clickable command chips, typed commands, Tab completion, ↑/↓ history, Ctrl+L / Ctrl+C. Added `/resume` (September 2026 v3 PDF) and a `resume` command.
- Backburner (Yegor's call, not on the site yet): a `raptorhacks` project entry. Draft copy: "RaptorHacks 2026 — Montgomery College's hackathon ('Hack the Planet'): ~100 students in teams of 2–4 across 7 tracks, Demo Day April 11, 2026 at the Germantown campus" + https://raptorhacks.com. Missing: Yegor's role and what he built/ran. Add to `PROJECTS` when he decides.
- The wins counter is `data-count="5"` per Yegor (5 podium finishes). Only three are itemised in `COMPETITIONS` (1st PICMC/MAGIC CTF 18, 2nd Lockheed Martin CyberQuest, 3rd VelocityX) because the resume lists only those; the `ctf` output is labelled "selected" for that reason. Ask him for the other two to complete the list.
- `WRITEUPS` is empty by design; the `writeups` command shows a "coming soon" message until entries are added.
- LinkedIn profile (linkedin.com/in/yegorkryvenka) could not be read from this machine (auth wall); content was taken from the September 2026 resume.
