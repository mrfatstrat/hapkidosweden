# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Public website for the Swedish section of World Kido Federation (hapkidosweden.se). The site promotes Hapkido martial arts, links to all Swedish member clubs, and showcases promotional material. See `PRD.md` for full requirements.

## Tech Stack

- **HTML**: Static HTML files with no templating
- **CSS**: Tailwind CSS via CDN (`https://cdn.tailwindcss.com`)
- **Fonts**: Google Fonts (Inter for body text, Noto Sans KR for Korean characters)
- **No build process**: Files are served directly without compilation

## Development Workflow

- **`index.html`** is the live published landing page. **Never modify it** unless explicitly told to.
- **`index_wip_N.html`** (e.g. `index_wip_1.html`) are working files for changes under review. All development happens here.
- WIP pages are not linked from `index.html` — they are only reachable by direct URL for sharing with reviewers.
- Once a WIP page is approved, it replaces `index.html`.
- If multiple WIP versions are needed, increment the number (`index_wip_2.html`, etc.).
- Use Chrome DevTools MCP to verify pages and debug problems both locally and on the published URL.
- Open HTML files directly in a browser to preview. No local server or build step required.

## File Structure

- `index.html` - Live published landing page (do not edit without explicit instruction)
- `index_wip_1.html` - Current working file

## Design Conventions

- Uses Tailwind utility classes for all styling
- Custom CSS classes defined in `<style>` block: `.korean-font`, `.hero-gradient`, `.section-spacing`, `.gallery-img`, `.social-icon`
- Color scheme: white background, gray-900 text, red-600 accents
- Typography: uppercase headings with wide letter-spacing, small font sizes for labels (text-[10px], text-[9px])
