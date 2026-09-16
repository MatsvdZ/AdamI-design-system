# AdamI Design System

Het volledige AdamI design system (v1), vastgelegd na de kickoff van de website-redesign (september 2026).

## Inhoud

- **`design-system.html`** — het volledige brandbook als losstaande pagina: open 'm in een browser voor kleuren, typografie, spacing, elevation, grid, iconen, buttons, forms, cards, beeldtaal, logo-richtlijnen (incl. don't-regels en co-branding), favicon/app-icon-specificatie en voice & tone.
- **`tokens/design-tokens.json`** — alle tokens (kleur, spacing, radius, typography, shadow, grid) in Tokens Studio-formaat (twee sets: `primitives` + `semantic`), rechtstreeks importeerbaar in Figma via de Tokens Studio-plugin.
- **`tokens/tokens.css`** — dezelfde tokens als CSS custom properties, klaar om te importeren in code (`:root { --color-navy: ...; }`).
- **`assets/logos/`** — de 6 officiële logo-bestanden als losse PNG's: wordmark, icon en volledige lockup (met "AI Consultancy"-tagline), elk in een navy-versie (lichte achtergrond) en een reversed/light-versie (donkere achtergrond).
- **`decisions.md`** — de beslissingenlog: welke keuzes zijn gemaakt, en waarom.

## Kernpalet

| Token | Hex | Rol |
|---|---|---|
| Navy | `#163172` | Primaire tekst, headings |
| Ink | `#081525` | Donkerste vlak |
| Cobalt | `#1E56A0` | Links, secundaire accenten |
| Sky | `#D6E4F0` | Kaart-/sectie-oppervlakken |
| Ember | `#C76607` | CTA/highlight — spaarzaam gebruiken |
| Background | `#FAFCFD` | Pagina-achtergrond |

Font: **Montserrat** (headings + body, 400/600/700), eyebrows/labels in **IBM Plex Mono** (500, uppercase, tracked).

## Gebruik

- Documentatie bekijken → open `design-system.html`.
- Tokens gebruiken in code → importeer `tokens/tokens.css`.
- Tokens gebruiken in Figma → importeer `tokens/design-tokens.json` via de Tokens Studio-plugin.
- Logo's gebruiken → pak het juiste bestand uit `assets/logos/` (zie logo-regels in `design-system.html`: wordmark voor nav desktop/tablet, icon voor nav mobiel, volledige lockup alléén in de hero).

## Live / bewerkbare versie

De actuele canvas-versie (met wijzigingsgeschiedenis) staat hier: https://claude.ai/artifact/3RYqhpCmJuugnvnfmLDVau

---
Gegenereerd met Claude — laatst bijgewerkt 16 september 2026.
