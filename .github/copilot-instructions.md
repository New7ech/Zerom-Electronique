# Zerom Electronique - AI Agent Instructions

## Project Overview
**Zerom Electronique** is a French-language e-commerce website for electronics and accessories. It's a portfolio project using vanilla HTML/CSS/JavaScript with Bootstrap framework for responsive design.

## Architecture & Key Files

### Core Pages (HTML)
- **index.html** - Homepage with banner carousel slider
- **computers.html** - Computer products catalog
- **mans_clothes.html** - Mobile phones/accessories (mapped to "Téléphones")
- **womans_clothes.html** - Other accessories (mapped to "Autres Accessoires")
- **contact.html** - Contact/inquiry form

All pages share identical navigation header structure with sidebar menu and responsive layout.

### Critical Patterns

#### Navigation & Layout
- **Sidebar Navigation**: Controlled via `openNav()` and `closeNav()` JS functions in [custom.js](../js/custom.js#L1)
- **Header Structure**: Common across all pages - contains logo, search, user, and cart icons
- **Language**: French (meta lang="fr") - all UI text and labels are in French
- **Mobile First**: Uses Bootstrap grid system with responsive CSS breakpoints in [responsive.css](../css/responsive.css)

#### JavaScript Dependencies & Patterns
- **jQuery-based**: Heavy reliance on jQuery plugins (not vanilla JS)
- **Key plugins** used in [custom.js](../js/custom.js):
  - **OwlCarousel** - Product/banner sliders
  - **MeanMenu** - Mobile menu handling
  - **NiceScroll** - Custom scrollbars
  - **Preloader** - Fade out loader after 1500ms
  - **Bootstrap tooltips** - Data-toggle="tooltip" elements
- **Selector patterns**: Most functionality uses `$(document).ready()` with jQuery selectors

#### CSS Architecture
- **Base fonts**: Poppins (main), Rajdhani, custom Baloo Chettan font
- **Color scheme**: Gray text (#666666), dark headings (#111111)
- **Transition effects**: Global 0.5s ease transitions on all elements (`transition: ease all 0.5s`)
- **Responsive breakpoints**: Handled via Bootstrap grid (col-md-4, col-md-12, etc.)

## Common Development Tasks

### Adding Product Cards
1. Create HTML structure using Bootstrap grid: `<div class="col-md-4">` (3-column layout common)
2. Add image and price sections within product card divs
3. Apply product-specific CSS classes from [style.css](../css/style.css)
4. Ensure images are placed in [images/](../images/) folder

### Modifying Navigation
- Update sidebar menu links in `<div id="mySidenav">` (same in every HTML file)
- Function calls: `openNav()` (hamburger menu open), `closeNav()` (close)
- All pages must maintain identical nav structure for consistency

### Adding Forms
- Contact page uses standard form structure
- Validate via jQuery: [jquery.validate.js](../js/jquery.validate.js) is included
- Form submission typically requires custom JS handlers in [custom.js](../js/custom.js)

## Important Conventions

### Image Management
- All product/site images in [images/](../images/) folder
- Icon files: `*-icon.png` naming convention (user-icon.png, search-icon.png, etc.)
- Product images: `img-*.png` or descriptive names (laptop-img.png, computer-img.png)

### CSS Organization
- Main custom styles in [style.css](../css/style.css) (979 lines)
- Responsive overrides in [responsive.css](../css/responsive.css)
- Bootstrap utilities supplemented with custom classes
- Do NOT directly modify Bootstrap files - extend with custom CSS

### HTML Structure
- All pages: `<!DOCTYPE html>` with `<html lang="fr">`
- Always include full meta viewport tags for mobile responsiveness
- CSS load order: Bootstrap → style.css → responsive.css
- JS load order: jQuery → plugins → custom.js (at end before closing body)

## External Dependencies (via CDN/Libs)
- Bootstrap CSS/JS (minified versions)
- Font Awesome 4.0.3 (from netdna)
- Google Fonts (Poppins)
- jQuery 3.0.0 + plugins
- FancyBox 2.1.5 (lightbox)
- Gijgo (likely for date picker)

## Debugging Tips
- **Preloader not disappearing?** Check the 1500ms timeout in [custom.js](../js/custom.js#L15)
- **Menu not working?** Verify openNav/closeNav function exists and sidebar menu ID is "mySidenav"
- **Carousel not sliding?** Check OwlCarousel initialization in [custom.js](../js/custom.js#L80+)
- **Mobile layout broken?** Inspect [responsive.css](../css/responsive.css) and Bootstrap grid structure

## File Structure Quick Reference
```
├── *.html              (5 page files, all share nav structure)
├── css/                (style.css + Bootstrap + plugins)
├── js/                 (jQuery, plugins, custom.js)
└── images/             (product/icon images)
```
