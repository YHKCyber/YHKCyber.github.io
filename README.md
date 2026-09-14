# yhkcyber.github.io

Personal link page for Yegor H. Kryvenka, styled as a terminal. Boots with `whoami` and `help`; the command buttons and the live prompt both run the same small command set (`projects`, `writeups`, `ctf`, `github`, `ncl`, `credly`, `linkedin`, plus `ls`, `cat`, `open`, `clear`).

## Stack

One static `index.html` — vanilla HTML, CSS and JavaScript, no build step. Deployed by GitHub Pages from `main`.

## Editing content

Everything shown by the terminal lives in `index.html`:

- The `whoami` block (name, role, education, org, cert, wins counter) and the `help` block are static HTML near the top of `<body>`. The wins counter is the `data-count` attribute on `.counter`.
- Projects, write-ups, competition results and links are the `PROJECTS`, `WRITEUPS`, `COMPETITIONS` and `LINKS` arrays at the top of the `<script>`. Add a write-up by pushing `{ slug, title, date, url, tags }` onto `WRITEUPS`; the empty-state message disappears automatically.

## Resume

`/resume` redirects to the latest PDF in `resume/`. To publish a new version, drop the new PDF into `resume/` and update the filename in `resume/index.html` (it appears three times). Old versions can stay for stable links.

## Local preview

```bash
python3 -m http.server 8000
```

then open http://localhost:8000.

## Credits

Font: [JetBrains Mono](https://www.jetbrains.com/lp/mono/) via Google Fonts. Built in part with Claude by Anthropic.

## License

Personal use only.
