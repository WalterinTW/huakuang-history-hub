# AGENTS.md

## Project goal
Build a static website hub for Huakuang Temple history experiments.

This repository is a parent-level website hub.
It has:
- one new top-level homepage
- two existing child pages:
  - `version-a/`
  - `version-b/`

The top-level homepage should introduce the two versions and link into them clearly.

## Important working rules
- Read this file before doing any work.
- Treat this repository as the source of truth for this task.
- Do not redesign `version-a` and `version-b` from scratch.
- Preserve the existing visual identity and internal content of both child pages as much as possible.
- Only make minimal necessary fixes inside child pages, mainly for path correctness and parent-level integration.
- The main new work is the new parent homepage.

## Scope of this task
Build a new top-level homepage for this repo that:
1. introduces the purpose of this hub
2. explains that there are two existing history-page versions
3. provides clear entry links to:
   - `version-a/`
   - `version-b/`
4. feels visually consistent with the existing Buddhist / dignified style
5. works well on desktop and mobile
6. is ready for GitHub Pages deployment

## Child page handling
The folders `version-a/` and `version-b/` already contain working static sites.

You may:
- inspect them
- fix broken relative paths if needed
- fix broken asset references if needed
- add a simple back-link from each child page to the new top-level homepage if appropriate

You must not:
- rewrite their full content
- replace their design entirely
- change their core structure unless required for path fixing

## Path rules
This repository will be deployed as a GitHub Pages project site.

Therefore:
- all links must use relative paths
- all asset paths must use relative paths
- avoid absolute-root paths like `/assets/...`
- verify that `version-a/` and `version-b/` still work correctly when opened from this parent repo structure

## Parent homepage requirements
The new top-level homepage should include:
- Hero section
- Short introduction to the history experiment
- Two clear cards or sections:
  - Version A: 摘要導覽式
  - Version B: 短介紹＋稍詳細內容
- A short explanation of the difference between the two versions
- Clear buttons linking to:
  - `version-a/`
  - `version-b/`

## Visual direction
Take visual inspiration from a calm Buddhist cultural website style:
- dignified
- serene
- restrained
- readable
- historical atmosphere
- elegant whitespace
- no flashy animation
- no strong commercial feeling

## Technical requirements
- Static site only
- Output files at repo root:
  - `index.html`
  - `style.css`
  - `script.js`
- Use semantic HTML
- Keep code beginner-friendly
- Keep layout responsive
- Prefer simple maintainable structure over clever complexity

## Deliverable checklist
Before finishing, verify:
1. root homepage loads correctly
2. root homepage links correctly to `version-a/`
3. root homepage links correctly to `version-b/`
4. `version-a/` assets still load
5. `version-b/` assets still load
6. no broken relative paths remain
7. site is suitable for GitHub Pages