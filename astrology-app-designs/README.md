# Akash — Astrology App Design Templates

Three visual directions for a cross-platform (iOS + Android) astrology app, 4 screens each.
Open `index.html` in a browser to see all 12 screens side by side. Each screen is a standalone,
clickable HTML mock in `screens/`.

| Template | Mood | Type | Core colours | Screens |
|---|---|---|---|---|
| **01 · Obsidian & Gold** | Dark luxury, editorial | Instrument Serif + Inter | `#09090F` `#F3EEE4` `#A9A4B8` `#E2C389` | Welcome, Today, Birth chart, Daily reading |
| **02 · Aurora Bento** | Bold, playful, social (Gen Z) | Unbounded + Manrope | `#0E0B1F` `#D4FF4F` `#8B8BFF` `#FF8A65` `#FFB3E1` | Pick your sign, Home bento, Compatibility, Daily tarot |
| **03 · Pearl Vedic** | Light, calm, Jyotish-first | Fraunces + Plus Jakarta Sans | `#F1F2F6` `#FFFFFF` `#12142B` `#E8622A` | Birth details, Home & Panchang, Janam Kundli, Consult |

## Modern UI elements used

- Frosted-glass cards, floating pill tab bar, raised AI action button
- Bento grid layouts, story rings, streak badge
- Energy / score rings, progress bars, stacked element-balance bar
- Natal chart wheel (Western) and North-Indian Kundli chart (Vedic)
- Live Panchang card with sun-arc, Rahu Kaal / Abhijit timeline, Dasha progress
- Venn-diagram compatibility score, fanned tarot deck
- Audio horoscope player, AI "Ask Akash" composer with suggestion chips
- Wallet balance, live session banner, astrologer marketplace cards
- Bilingual toggle (EN / हिं)

## Cross-platform spec

- Base frame **390 × 844** (iPhone 15 / Pixel 8 class); layouts flex across 360–430 pt widths.
- Safe areas: **54 pt** top inset, **34 pt** bottom home-indicator / gesture bar.
- Touch targets **≥ 44 pt (iOS) / 48 dp (Android)**.
- **8-pt** spacing grid; corner radii 18–28 px for cards, full pills for buttons.
- No platform-only chrome, so one Flutter or React Native codebase renders identically on both.
- All fonts are free Google Fonts; zodiac/planet glyphs use Noto Sans Symbols with text presentation (`U+FE0E`) so they never turn into emoji.

## Note on content

Names, chart positions, Panchang timings and prices are illustrative sample data.
Connect an ephemeris / Panchang API before shipping.
