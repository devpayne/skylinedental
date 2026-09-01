# Skyline Dental — Website

A modern, animated redesign of skylinedentistry.net for Dr. Aaron Olson's practice in Brigham City, UT. Plain HTML/CSS/JS — no build step, deploys straight to Netlify.

## Structure

- `index.html` — all page content/sections
- `css/style.css` — design tokens, layout, animations
- `js/main.js` — scroll reveal, sticky nav, testimonial carousel, count-up stats, mobile menu
- `netlify.toml` — Netlify build/publish + basic security headers

## Before going live

- **Photos**: replace the placeholder "DR. OLSON" block in the About section (`.about-photo-placeholder` in `index.html`) with a real portrait, and consider adding office photos near the Office section.
- **Hours**: the current site content didn't specify office hours — add them to the Office section once confirmed.
- **Social links**: `#` placeholders for Facebook/Instagram in the Office section and footer — swap in the real profile URLs.
- **Map**: the embedded Google Map uses the practice address; double check the pin looks correct once live.

## Contact form

The appointment form uses [Netlify Forms](https://docs.netlify.com/manage/forms/setup/) (`data-netlify="true"`) — no backend needed. Once deployed on Netlify, submissions show up automatically under Site settings → Forms. You can add an email notification there so submissions land in an inbox.

## Deploying

1. Push this repo to GitHub (already set up at `devpayne/skylinedental`).
2. In Netlify: **Add new site → Import an existing project → GitHub** → select this repo.
3. Build command: none needed. Publish directory: `.` (already set in `netlify.toml`).
4. Deploy — Netlify will auto-redeploy on every push to `main`.
