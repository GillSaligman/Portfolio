# Gill Saligman's portfolio site

Static site served by GitHub Pages at gillsaligman.github.io/Portfolio. No build step: plain HTML + one stylesheet.

## Design
- Clean "engineering drawing" style. All styling lives in `assets/css/site.css`. Do not reintroduce the old HTML5 UP template (`assets/css/main.css`, jQuery scripts); those files are unused leftovers.
- Fonts: IBM Plex Sans (body) and IBM Plex Mono (labels, numbers) from Google Fonts.
- Colors are CSS variables on `:root` with a dark-mode override. Use the tokens, never hard-coded colors.
- Keep it plain and human: no stat boxes, big-number rows, or decorative badges. Gill dislikes anything that looks AI-generated.
- Footer on every page is a simple `.site-footer` line with contact info.

## Structure
- `index.html`: homepage. Projects are `<article class="project">` rows with `.specs` lists, most recent first.
- Project pages (`nauticus.html`, `robotarm.html`, `frc.html`, `moa.html`, and the Ministry of Awe sub-pages `typewriter.html`, `phone-system.html`, `ear-teller.html`, `watching-table.html`) share one layout: site header, `.page-head`, content inside `.legacy`, `.site-footer`. `moa.html` is hand-built with `.build` sections instead of `.legacy`.
- To add a project page, copy `typewriter.html` and replace the content inside `<div class="legacy">`.

## Images
- Originals are in `images/` (some are large .MOV videos). Web-sized copies used by the homepage are in `images/web/` (JPEG, max 1400px). Make a web-sized copy for any new photo. Videos live in `images/web/video/` as H.264 .mp4 (phone .MOV files are HEVC and do not play in Chrome), each with a .jpg poster frame.
- `images/images/` is a duplicate folder from an old upload and is not used.

## Facts to keep consistent with the resume
- Name: Gill Saligman. Email jsaligman@gmail.com, phone 610-316-5180.
- Vulcan Spring (Jun 2026–present): coiler rebuilt to 4,200 parts/hr vs 3,500 target; fixed decade-old double-press fault; machine vision part checker. No photos yet.
- Ministry of Awe (Aug 2025–Apr 2026), 7-DOF arm senior design (Sep 2024–Jun 2025), Nauticus Robotics (Sep 2023–May 2024).
