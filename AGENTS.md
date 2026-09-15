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

- 2026-09-15: `projects` now holds exactly one entry — the Raspberry Pi bastion host home-lab build (`bastion`), written from Yegor's draft write-up (`WriteupServerUpgradingProject.docx`, not in the repo). Work-experience bullets and club leadership are NOT projects and must not go back into `PROJECTS`. The public description deliberately omits the bastion's SSH port and internal LAN addresses.
- `ctf` shows wins only (Blue Team Con Last Minute CTF 2026 1st of ~60, PICMC Cyber Challenge 2026 1st, MAGIC CTF 18 1st — two separate competitions, Lockheed Martin CyberQuest 2nd, VelocityX 3rd, plus NCL 99th percentile) — no team/leadership rows; the site is deliberately less recruiter-tailored than the resume. Counter is `data-count="5"`.
- `/resume` points at the September 2026 v4 PDF (`resume/Yegor-Kryvenka-Resume-2026-09-v4.pdf`); v3 was removed.
- Backburner (Yegor's call, not on the site): a RaptorHacks entry. The v4 resume now states the role — "Co-organized and hosted RaptorHacks 2026, an intercollegiate hackathon at Montgomery College, building a real-time project submission and judging platform while coordinating a panel of judges, faculty, and an FDA guest speaker across tracks including dedicated cybersecurity penetration testing." Site: https://raptorhacks.com. Add to `PROJECTS` only if he asks.
- `WRITEUPS` is empty; the `writeups` command says the bastion write-up is first up and links to the project. When the polished write-up exists, host it (e.g. `writeups/bastion.html` or a PDF) and add `{ slug: 'bastion', title, date, url, tags }`.
- Tab completion and ↑/↓ history still work in the prompt but are no longer advertised in the help text (Yegor asked for the hint removed).
- LinkedIn profile (linkedin.com/in/yegorkryvenka) is auth-walled from this machine; content comes from the resume and the write-up.
