# resume

[![Build Resume](https://github.com/avery-wagner/resume/actions/workflows/build.yml/badge.svg)](https://github.com/avery-wagner/resume/actions/workflows/build.yml)

My resume, in LaTeX, version-controlled.

Built on [AltaCV](https://github.com/liantze/AltaCV) by LianTze Lim.

## Compile

<!--**Overleaf (no local setup):**
1. New Project → Blank Project, paste in `AW_Res.tex` and `altacv.cls`
2. Menu → paper size → Letter
3. Recompile-->

**Locally** (needs a LaTeX distribution with `latexmk`):
```sh
latexmk -pdf AW_Res.tex
```

`AW_Res.pdf` isn't tracked in git — it's a build output, not source. CI (`.github/workflows/build.yml`) compiles it on every push and pull request and attaches the result as a downloadable workflow artifact (Actions tab → latest run → Artifacts), so there's always a fresh copy without baking old versions into git history.
