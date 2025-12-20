# London Trip Presentation - Handover Document

## Project Overview

A mobile-first HTML presentation for a London trip itinerary (24 Dec 2025 - 1 Jan 2026). The presentation is intended for Indonesian guests visiting London, so all content is in Indonesian.

## Files

- `london_trip_presentation.html` - Single-file HTML presentation (self-contained)

## Tech Stack

- **Swiper.js v11** (CDN) - Touch-enabled slide navigation
- **Google Fonts** - Playfair Display (headings), Inter (body)
- **Vanilla CSS** - No preprocessors
- **Unsplash** - Background images via URL parameters

## Design Decisions

- Single HTML file for easy sharing/hosting
- Mobile-first (100vh/100dvh viewport)
- Dark theme (#0a1628 base) with image backgrounds
- Gradient overlays on background images for text readability
- Color-coded badges: red (default), blue, gold, green, purple
- Yellow (#ffc107) for costs and travel times
- Light blue (#7dd3fc) for hyperlinks
- Content area scrollable within each slide

## Slide Structure (17 slides)

1. Title slide (centered layout)
2. Overview/Ringkasan
3. Day 1 - 24 Dec (Rabu) - Windsor Castle, Central London Drive
4. Day 2 - 25 Dec (Kamis) - Christmas Day - South Bank, Tower Bridge, Chinatown
5. Day 3 - 26 Dec (Jumat) - Boxing Day - Covent Garden, Oxford Street, Musical
6. Day 4 - 27 Dec (Sabtu) - Borough Market, Tower of London, Portobello, London Eye
7. Day 5 - 28 Dec (Minggu) - Snow Centre, St Albans
8. Day 6 - 29 Dec (Senin) - Hyde Park, Winter Wonderland, Harrods
9. Day 7 - 30 Dec (Selasa) - Uber day - Buckingham, Museums
10. Day 8 - 31 Dec (Rabu) - NYE
11. Day 9 - 1 Jan 2026 (Kamis) - Return flight
12. Booking priorities list
13. Catatan Penting - Cuaca & Pakaian (Weather & Clothing)
14. Catatan Penting - Kesehatan & Obat (Health & Medicine)
15. Catatan Penting - Keuangan & Internet (Finance & Connectivity)
16. Catatan Penting - Barang Penting (Essential Items)
17. Closing slide (centered layout)

## Trip Details

- **Dates**: 24 December 2025 - 1 January 2026
- **Group**: 5 adults, 1 teen, 1 toddler
- **Hotel**: Staybridge Suites Heathrow Bath Road (5 min from airport)
- **Transport**: Driver from Sheffield for days 1-6, Uber for days 7-8
- **Key bookings needed**: West End Musical (26 Dec), Winter Wonderland (29 Dec), Windsor Castle, Tower of London, London Eye, Snow Centre, Sky Garden

## Recent Changes

1. Corrected dates from 2024-2025 to 2025-2026
2. Swapped Day 4 (Ski) and Day 5 (Borough/Tower) so Portobello Market lands on Saturday
3. Changed title from "Panduan Perjalanan Lengkap" to "Panduan Perjalanan Singkat"
4. Removed budget estimate box from overview slide
5. Added hyperlinks to venues and items of interest throughout
6. Added disclaimer on opening slide
7. Added dinner entries (TBD) to Days 24, 25, 27, 28, 29
8. Made content card extend full height to fix mobile scroll clipping issue

## CSS Classes Reference

- `.swiper-slide` - Base slide container
- `.title-slide` - Centered layout for title/closing slides
- `.slide-bg` - Background image container with gradient overlay
- `.slide-content` - Scrollable content area
- `.day-badge` - Colored pill badges (variants: `.blue`, `.gold`, `.green`, `.purple`)
- `.info-card` - Content cards (variants: `.highlight`, `.success`, `.warning`, `.purple`)
- `.timeline-item` - Time + content row
- `.time` - Time badge (variant: `.red`)
- `.travel-time` - Yellow italic travel duration text
- `.hotel-times` - Departure/return time badges container
- `.cost` - Yellow cost text
- `.suggestion-grid` - 2-column grid for suggestions

## Known Considerations

- Background images load from Unsplash (requires internet)
- Swiper.js loads from CDN (requires internet)
- Some slides have lots of content and require scrolling on mobile
- Hyperlinks open in new tabs (`target="_blank"`)

## Hosting

Ready for GitHub Pages:
1. Rename to `index.html`
2. Upload to repository
3. Enable Pages from Settings

## User Preferences (for Claude Code)

- Avoid em dashes
- Keep sentence structure simple and brief
- Use bullets and numbered lists sparingly
- User codes primarily in Python
