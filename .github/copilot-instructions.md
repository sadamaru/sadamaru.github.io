# AI Agent Instructions for sadamaru.github.io

This document provides essential guidance for AI agents working with this portfolio website project.

## Project Overview

This is a personal portfolio website built with HTML, CSS, and JavaScript. The site uses:
- Bootstrap as the primary CSS framework
- jQuery for JavaScript functionality
- Various vendor libraries for animations and UI components

## Key Architecture Components

### 1. Asset Organization
- `assets/css/`: Core stylesheets including Bootstrap and custom styles
- `assets/js/`: JavaScript files including jQuery and custom scripts
- `assets/vendor/`: Third-party libraries and components
- `assets/img/`: Image assets including portfolio work samples

### 2. Theme System
The project implements a color theme system that allows users to switch between different color schemes:
- Theme colors: red (default), blue, green, orange, purple
- Theme switching is handled via CSS classes and JavaScript
- See the theme implementation in the config panel in `index.html`

### 3. Major Dependencies
- Bootstrap (v4+) for responsive layouts and components
- jQuery 3.5.1 for DOM manipulation and animations
- Various vendor libraries:
  - Owl Carousel for sliders
  - Animate.css for animations
  - Fancybox for image galleries
  - WayPoints for scroll animations
  - Isotope for portfolio filtering

## Development Workflows

### Local Development
1. No build process required - this is a static site
2. Serve the root directory using any static file server
3. Browser caching may need to be disabled during development

### File Structure Conventions
- Keep new style additions in `assets/css/virtual.css`
- Place new JavaScript functionality in `assets/js/minibar-virtual.js`
- Add new vendor libraries to `assets/vendor/`
- Store portfolio images in `assets/img/work/`

### Responsive Design
- The site uses Bootstrap's responsive grid system
- Test all changes at key breakpoints: 
  - Mobile: < 576px
  - Tablet: 576px - 992px
  - Desktop: > 992px

## Common Patterns and Practices

### Theme Color Management
When adding new themed elements:
1. Use the `.theme-{color}` classes for parent elements
2. Define color variations in each theme-specific CSS section
3. Reference example: Back-to-top button implementation in HTML/CSS

### JavaScript Initialization
New interactive components should:
1. Wait for document ready: `$(document).ready(function() { ... })`
2. Follow the initialization pattern in `minibar-virtual.js`
3. Use event delegation for dynamically added elements

## Integration Points
- Font icons: Uses Themify Icons - reference the pattern in existing elements
- Image galleries: Integrate with Fancybox for lightbox functionality
- Animations: Use combination of Animate.css classes and WOW.js for scroll reveals

Need any clarification or have specific sections you'd like me to expand upon?
