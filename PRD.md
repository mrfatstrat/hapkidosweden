# Product Requirements Document: Hapkido Sweden Website

## Overview

**Project**: Public website for the Swedish section of World Kido Federation
**Domain**: svenskhapkido.se
**Purpose**: Common landing site for all Swedish member clubs to promote Hapkido and attract new members

## Goals

1. Promote Hapkido as a martial art to the Swedish public
2. Provide a central hub linking to all member clubs
3. Showcase promotional material (photos, videos)
4. Connect visitors with the global World Kido Federation
5. Make it easy for interested people to find and contact a local club

## Target Audience

- People in Sweden interested in martial arts or self-defense
- Parents looking for activities for their children
- People searching for Hapkido specifically
- International visitors researching Swedish Hapkido (secondary)

## Language

Swedish only

## Hosting

GitHub Pages (free static hosting)

## Core Features

### 1. About Hapkido Section
- Explain what Hapkido is according to WKF interpretation
- Cover the philosophy (Hap, Ki, Do)
- Highlight key aspects: self-defense, training, community, personal development
- Reference traditional Korean martial arts heritage

### 2. Member Clubs Directory
- List all affiliated clubs with:
  - Club name
  - Location/city
  - Link to club website
- Design must support adding new clubs easily
- Current clubs:
  - Nordic Hapkido Club (Skellefteå)
  - Kampsportshuset (Stockholm)
  - Hanmoosa (Linköping)
  - Lidköping Kampsport (Lidköping)

### 3. Media Gallery
- Photo gallery showcasing training, events, techniques
- Embedded videos (YouTube)
- Should be easy to add new media

### 4. World Kido Federation Connection
- Dedicated section about WKF affiliation
- Display WKF and Hanminjok logos
- Link to worldkidofederation.com
- Explain international certification and recognition

### 5. Contact Information
- Email contact: worldkido.se@gmail.com
- Social media links (Facebook, Instagram, TikTok, YouTube)
- Clear call-to-action for joining or asking questions

### 6. Navigation
- Sticky header with logo and navigation
- Smooth scroll to sections
- Mobile-friendly hamburger menu (if needed)

## Technical Requirements

### Responsive Design
- Mobile-first approach
- Must look good on:
  - Mobile phones (320px - 480px)
  - Tablets (768px - 1024px)
  - Desktop (1024px+)
- Touch-friendly tap targets on mobile

### SEO Optimization
- Semantic HTML5 structure
- Proper heading hierarchy (h1, h2, h3)
- Meta tags: title, description, keywords
- Open Graph tags for social sharing
- Alt text on all images
- Fast loading times
- Structured data (Organization, LocalBusiness)

### Performance
- Optimize images (WebP format, appropriate sizes)
- Minimize external dependencies
- Target < 3 second load time on mobile

### Accessibility
- Sufficient color contrast
- Keyboard navigation support
- Screen reader friendly

## Design Requirements

### Visual Style
- Modern, clean aesthetic
- Traditional Korean martial arts references:
  - Korean characters (한글) as decorative elements
  - Color palette inspired by Korean aesthetics
- Color scheme:
  - Primary: White/light backgrounds
  - Text: Dark gray (#1a1a1a)
  - Accent: Red (#dc2626) - traditional martial arts color
  - Secondary accents: Subtle grays

### Typography
- Body: Clean sans-serif (Inter)
- Korean characters: Noto Sans KR
- Uppercase headings with letter-spacing for modern feel

### Imagery
- High-quality photos from member clubs
- Action shots of training
- Hero image setting martial arts tone

## Tech Stack

- **HTML5**: Semantic markup
- **Tailwind CSS**: Via CDN for simplicity
- **No JavaScript framework**: Keep it simple, vanilla JS if needed
- **No build process**: Direct file editing for easy maintenance

## Content Structure

```
1. Hero Section
   - Korean characters (합기도)
   - "Hapkido" headline
   - Tagline
   - CTA button to clubs section

2. About Hapkido
   - Description of the martial art
   - What training includes
   - Embedded video (optional)

3. Philosophy
   - Hap (합) - Harmony
   - Ki (기) - Energy
   - Do (도) - The Way

4. Member Clubs
   - Grid of club cards
   - Each with city, name, link

5. Gallery
   - Photo grid
   - Video embeds

6. World Kido Federation
   - Logos
   - Description of affiliation
   - Link to WKF website

7. Contact
   - Email
   - Social media links

8. Footer
   - Copyright
```

## Maintenance

### Adding a New Club
Edit the clubs section in `index.html`:
```html
<div class="p-8 bg-white border...">
    <p class="text-red-600...">City Name</p>
    <h4 class="font-bold...">Club Name</h4>
    <a href="https://club-website.com">Besök hemsida</a>
</div>
```

### Adding Photos
Add new `<img>` elements to the gallery grid with appropriate URLs.

### Adding Videos
Embed YouTube iframes in the designated video section.

## Success Metrics

- Website loads in < 3 seconds on mobile
- Passes Google Lighthouse audit (Performance, SEO, Accessibility > 90)
- Club websites receive referral traffic from the site
- Contact email receives inquiries from potential members

## Future Considerations (Out of Scope)

- English language version
- Event calendar
- News/blog section
- Online membership registration
- CMS integration

## Timeline

Phase 1 (Current): Single-page static site with all core features
