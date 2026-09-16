# AdamI Design System — v1 beslissingen (kickoff sept 2026)

Vastgelegd na de kickoff-meeting. Volledig uitgewerkt als canvas: https://claude.ai/artifact/3RYqhpCmJuugnvnfmLDVau

## Kleuren

| Kleur | Hex | Rol |
|---|---|---|
| Navy | #163172 | Primaire tekst, headings, outline-knoppen |
| Ink | #081525 | Donkerste vlak — footer, donkere secties |
| Cobalt | #1E56A0 | Links, secundaire accenten, focus states |
| Sky | #D6E4F0 | Kaart- en sectie-oppervlakken |
| Ember | #C76607 | CTA/highlight — spaarzaam gebruikt, grote vlakken |
| Ember CTA (afgeleid) | #A6560A | Alleen voor solide button-fills — Ember zelf geeft met witte tekst ~3,9:1 contrast (net niet AA); deze verdiepte variant haalt ~5,3:1 |
| Background | #FAFCFD | Pagina-achtergrond — de echte waarde van de live site, geen puur wit |
| Success (semantisch) | #1E7145 | Bevestigingen — los van het accent |
| Error (semantisch) | #B3261E | Foutmeldingen, formuliervalidatie |

Daarnaast een laag ondersteunende/afgeleide kleuren (surface soft #EEF4FA, border #DBE4EF, text-muted #4D6198, neutral-ramp 200/400/600/800) — geen eigen merkkeuzes, maar wel echte tokens die door het hele systeem gebruikt worden. Code-bg/code-text zijn bewust puur voor de documentatiepagina zelf, niet onderdeel van het site-palet.

## Typografie

- **Montserrat**: headings (600/700) én body copy (400 Regular).
- **IBM Plex Mono**: alleen nog eyebrows/labels (500, uppercase, tracked).
- Bewust beperkte schaal: display (hero only), h2, h3, body, small, label — elk met een desktop- en mobile-waarde.

## Grid, elevation & iconen

- **Grid**: 12 kolommen desktop (≥1024px), 8 tablet (≥640px), 4 mobiel; max content-breedte 1280px, gutter 24px overal.
- **Elevation**: drie navy-getinte schaduwniveaus (sm/md/lg) voor hover, dropdowns en modals — geen puur zwart.
- **Iconen**: één lijnstijl, 24×24 grid, 1,75px lijndikte, afgeronde uiteinden, altijd in tekstkleur. Social/platform-iconen: altijd het officiële merkicoon van het platform zelf, ongewijzigd.
- **Formulieren**: labels hergebruiken de label/eyebrow-stijl; focus = cobalt ring, error = de semantische errorkleur (nooit Ember).

## Beeldtaal

- **Team**: echte foto's, behandeld met een navy/ember- of navy/cobalt-duotone zodat ze bij het blauwe palet blijven passen.
- **Cases**: logo-forward — het klantlogo is de identificatie, geen (perse) echte klantfoto's.

## Logo

Drie lockups, elk in een navy-versie (lichte achtergrond) en een reversed versie (donkere/navy achtergrond): Wordmark (nav desktop/tablet), Icon (nav mobiel), Volledige lockup met tagline (hero only, nooit in nav). Plus: minimale vrije ruimte, don't-regels, co-branding-regel voor naast een klantlogo, en favicon/app-icon-specificatie (32/180/512px).

## Voice & tone

Toon: zelfverzekerd, precies, licht technisch — nooit salesy. Concrete cijfers, CTA's benoemen de daadwerkelijke volgende stap.

## Figma

Alle tokens staan als importeerbaar JSON-bestand (Tokens Studio-formaat, `tokens/design-tokens.json`). De live Figma-koppeling werkte niet in de sessie waarin dit is opgezet; zodra die hersteld is kan dit rechtstreeks als Figma Variables gesynchroniseerd worden i.p.v. via handmatige import.

## Homepage — hero

Drie schermvullende hero-richtingen uitgewerkt: https://claude.ai/artifact/GnTF5DKZ9Dq57Jw2UZTfhD

- **Optie A — Duna-stijl (aanbevolen)**: gelaagde bergsilhouetten (Navy/Ink) met een meer, Ember-zon als enige warme accent.
- **Optie B — Zachte lucht**: abstracte wolkenlucht (Sky → Cobalt gradient), Ember-gloed als zonsopkomst.
- **Optie C — Abstracte skyline**: platte skyline-silhouet bij schemering, Cobalt → Sky lucht, Ember-zon met stralenkrans.

Alle drie zijn zelfgebouwde SVG/CSS-illustraties (geen AI-gegenereerd beeld — beeldgeneratie was niet beschikbaar op het gekoppelde account). Keuze: nog te bevestigen (voorkeur ligt bij optie A).

## Nog open

- Definitieve keuze hero-richting bevestigen en de rest van de homepage bouwen.
- Layout van overige pagina's (cases, etc.).
- Live Figma-koppeling herstellen voor directe synchronisatie i.p.v. JSON-import.
- Figma-componentbibliotheek (buttons/forms/cards/logo's als echte componenten, niet alleen tokens).
