# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Public website for the Swedish section of World Kido Federation (svenskhapkido.se). The site promotes Hapkido martial arts, links to all Swedish member clubs, and showcases promotional material. See `PRD.md` for full requirements.

## Tech Stack

- **HTML**: Static HTML files with no templating
- **CSS**: Tailwind CSS via CDN (`https://cdn.tailwindcss.com`)
- **Fonts**: Google Fonts (Inter for body text, Noto Sans KR for Korean characters)
- **No build process**: Files are served directly without compilation

## Development

Open `index.html` directly in a browser to preview the site. No local server or build step required.

## File Structure

- `index.html` - Main website (current working version)
- `webpage-mockup_1.html` - Earlier mockup version (committed to git)

## Design Conventions

- Uses Tailwind utility classes for all styling
- Custom CSS classes defined in `<style>` block: `.korean-font`, `.hero-gradient`, `.section-spacing`, `.gallery-img`, `.social-icon`
- Color scheme: white background, gray-900 text, red-600 accents
- Typography: uppercase headings with wide letter-spacing, small font sizes for labels (text-[10px], text-[9px])
