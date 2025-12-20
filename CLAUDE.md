# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML travel guide for a London trip (December 24, 2025 - January 1, 2026). It's a single-page application that displays an interactive, swipeable itinerary designed primarily for mobile viewing.

## Technology Stack

- **Single `index.html` file** - all HTML, CSS, and JS in one file
- **Swiper.js v11** - horizontal swipe navigation between slides (loaded via CDN)
- **Google Fonts** - Playfair Display and Inter fonts
- **No build process** - static HTML, open directly in browser

## Development

To preview: open `index.html` in a browser, or use any local server (e.g., `python -m http.server`).

## Architecture

The page is structured as a series of Swiper slides:
- Title slide and overview
- Day-by-day itinerary (Days 1-9)
- Booking priority list
- Practical notes (weather, health, finance, essentials)
- Closing slide

Each slide has:
- Background image (Unsplash URLs)
- Gradient overlay for text readability
- Content cards with timeline items, info boxes, and travel times

## Key CSS Classes

- `.swiper-slide` - individual slide container
- `.slide-bg` - full-screen background image with gradient overlay
- `.slide-content` - scrollable content area
- `.info-card` - styled content boxes (variants: `.highlight`, `.success`, `.warning`, `.purple`)
- `.timeline-item` / `.time` - itinerary timeline entries
- `.day-badge` - colored day/category labels (variants: `.blue`, `.gold`, `.green`, `.purple`)
