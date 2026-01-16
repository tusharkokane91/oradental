# AGENTS.md

This file provides guidance to AI agents when working with code in this repository.

## Project Overview

- **Name**: Ora Dental Clinic Website
- **Type**: Static Website / Landing Page
- **Primary Language**: HTML, CSS, JavaScript (Vanilla)
- **Framework**: None (Pure static site - no build tools required)
- **Description**: Professional website for Ora Dental Clinic by Dr. Shivani Gujarathi Dagadu, located in Baner, Pune. Features clinic information, services, contact details, and Google Maps integration.

## Architecture & Structure

```
oradentalweb/
├── index.html          # Main HTML file (single-page website)
├── styles.css          # All CSS styles (responsive, mobile-first)
├── script.js           # JavaScript for interactivity & animations
├── assets/
│   └── logo.jpg        # Clinic logo (brown/gold branding)
└── AGENTS.md           # This file
```

**Architecture Pattern**: Single-page static website with section-based navigation. No server-side rendering or build process required.

## Technology Stack

### Frontend
- **HTML5**: Semantic markup with accessibility considerations
- **CSS3**: Custom properties (CSS variables), Flexbox, Grid, animations
- **JavaScript (ES6+)**: Vanilla JS for interactivity (no jQuery/frameworks)
- **Google Fonts**: Playfair Display (headings), Poppins (body)
- **Font Awesome 6.5**: Icon library via CDN

### External Integrations
- **Google Maps Embed**: Clinic location display
- **WhatsApp API**: Click-to-chat functionality
- **Tel/Mailto Links**: Direct phone/email contact

### No Build Tools Required
This is a pure static site - just open `index.html` in a browser or deploy to any static host.

## Development Guidelines

### Code Style & Conventions

**HTML**:
- Use semantic elements (`<section>`, `<nav>`, `<footer>`, etc.)
- Include appropriate ARIA labels for accessibility
- Keep consistent indentation (4 spaces)

**CSS**:
- Use CSS custom properties defined in `:root` for theming
- Follow mobile-first responsive approach
- Group styles by component/section with comment headers
- Color palette:
  - Primary (Brown): `#A0522D`
  - Accent (Gold): `#DAA520`
  - Background: `#FFF9F5`
  - Text: `#3D2914`

**JavaScript**:
- Use `const`/`let` (no `var`)
- Event delegation where appropriate
- Keep animations smooth (use `requestAnimationFrame` for counters)

### File Organization
- All styles in single `styles.css` (organized by section)
- All scripts in single `script.js`
- Images/assets in `assets/` folder

### Git Workflow
- Main branch: `main`
- Commit messages should be descriptive
- Remote: `git@github.com:tusharkokane91/oradental.git`

## AI Agent Instructions

### Project Context
- **Working Style**: Small business website - prioritize simplicity and maintainability
- **Focus Areas**: Visual appeal, mobile responsiveness, fast loading, SEO
- **Common Tasks**: Content updates, styling tweaks, adding new sections

### Command Preferences
- **File Operations**: All editable files are in root directory
- **Testing**: Open `index.html` directly in browser (`open index.html` on macOS)
- **No Build Process**: Changes are immediately visible on refresh

### Best Practices for This Project

1. **Keep it Simple**: No unnecessary frameworks or build tools
2. **Performance**: Minimize external dependencies, optimize images
3. **Mobile First**: Test responsive design on multiple screen sizes
4. **Accessibility**: Maintain ARIA labels, semantic HTML, good color contrast
5. **SEO**: Keep meta tags updated, use descriptive alt texts

### Content Updates
When updating clinic information:
- **Contact**: Phone `8766788271`, Email `oradental03@gmail.com`
- **Address**: Elliot 3rd Floor, Near Zudio Mall & ABZ Gate No.1, Veer Bhadra Nagar, Ganraj Chowk, Baner, Pune 411045
- **Google Maps**: Use provided embed code with Ora Dental Clinic marker
- **WhatsApp**: Links use `wa.me/918766788271` format

## Quick Reference

### Common Commands
- **View Site**: `open index.html`
- **Local Server**: `python3 -m http.server 8000` (then visit localhost:8000)
- **Git Push**: `git add -A && git commit -m "message" && git push`

### Deployment Options
1. **Netlify**: Drag & drop folder to netlify.com/drop
2. **GitHub Pages**: Enable in repo settings
3. **Surge**: `npx surge .`
4. **Vercel**: Connect GitHub repo

### CSS Variables Reference
```css
--primary: #A0522D;        /* Brown - buttons, headings */
--primary-dark: #8B4513;   /* Dark brown - hover states */
--accent: #DAA520;         /* Gold - highlights, badges */
--bg-light: #FFF9F5;       /* Off-white background */
--text-dark: #3D2914;      /* Main text color */
```

### Key Sections (by ID)
- `#home` - Hero section
- `#about` - About Dr. Shivani
- `#services` - Dental services grid
- `#contact` - Contact info & map

## Notes & Context

### Business Information
- **Clinic**: Ora Dental Clinic
- **Doctor**: Dr. Shivani Gujarathi Dagadu
- **Location**: Baner, Pune, Maharashtra, India
- **Services**: General dentistry, root canal, teeth whitening, braces, implants, pediatric dentistry, extractions, crowns & bridges

### Design Decisions
- **Color Scheme**: Derived from clinic logo (warm brown + gold)
- **Typography**: Elegant serif for headings (Playfair Display), clean sans-serif for body (Poppins)
- **Animations**: Subtle scroll animations, floating logo effect, counter animations
- **WhatsApp Float**: Prominent floating button for easy patient contact

### Future Enhancements to Consider
- Add testimonials/reviews section
- Add photo gallery of clinic
- Add online appointment booking form
- Add blog/dental tips section
- Multi-language support (Hindi/Marathi)

### Important Files to Backup
- `assets/logo.jpg` - Original clinic logo
- `index.html` - All content and structure
- `styles.css` - All visual styling
