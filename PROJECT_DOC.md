# SUM Accountants - Vacature Website
**Project:** Werken bij SUM Accountants Landingspagina
**Datum:** Januari 2026
**Type:** Single-page HTML vacaturewebsite

---

## 📋 Inhoudsopgave

1. [Project Overzicht](#project-overzicht)
2. [Bestandsstructuur](#bestandsstructuur)
3. [Kleurpalet](#kleurpalet)
4. [Pagina Structuur](#pagina-structuur)
5. [Contact Gegevens](#contact-gegevens)
6. [Video Content](#video-content)
7. [Aanpassingen Maken](#aanpassingen-maken)
8. [Git Geschiedenis](#git-geschiedenis)

---

## Project Overzicht

Moderne, responsieve vacaturewebsite voor SUM Accountants in Krimpen aan den IJssel. De pagina is ontworpen om professionals te werven die het verschil willen maken voor mkb-ondernemers.

**Kenmerken:**
- ✅ Single-page HTML met inline Tailwind CSS
- ✅ Responsive design (mobiel + desktop)
- ✅ Sticky navigatie met scroll effects
- ✅ YouTube video integratie
- ✅ WhatsApp contact knop (sticky)
- ✅ FAQ sectie met accordions
- ✅ Christelijke identiteit uitstraling

---

## Bestandsstructuur

```
werkenbijsum.nl/
├── index.html              # Hoofdpagina (alle content)
├── images/                 # Afbeeldingen
│   ├── antoinette.jpg
│   ├── DSC07674-3-team-overleg-staand-2048x942px.jpg
│   ├── DSC07699-twee-medewerkers-drinken-samen-koffie-focus-op-handen-en-koffiekopjes-2048x521px.jpg
│   ├── DSC07760-antoinette-voor-scherm-met-cijfers-2048x102px.jpg
│   └── DSC07791-antoinette-legt-uit-aan-team-2048x1365px.jpg
├── PROJECT_DOC.md          # Dit bestand
└── .git/                   # Git repository
```

---

## Kleurpalet

De website gebruikt CSS custom properties (variabelen) gedefinieerd in de `<style>` section:

```css
:root {
  --primary: #7C3AED;      /* Paars - primaire kleur */
  --secondary: #EC4899;    /* Roze - secundaire kleur */
  --accent: #F2C7DF;       /* Licht roze - accent kleur */
  --text: #1F2937;         /* Donker grijs - tekst */
}
```

**Gebruik:**
```html
<div class="bg-[var(--primary)]">       /* Primaire achtergrond */
<div class="text-[var(--secondary)]">   /* Secundaire tekst */
<div class="border-[var(--accent)]">    /* Accent border */
```

---

## Pagina Structuur

### 1. Header & Navigatie
**Locatie:** `<header>` (regels ~140-180)

**Elementen:**
- Logo (Zwart AND Wit versie)
- Desktop navigatie met links
- Mobile hamburger menu
- Sticky bij scrollen

**Navigatie items:**
- MISSIE → `#missie`
- JOUW ROL → `#rol`
- DE MATCH → `#match`
- ONS AANBOD → `#voordelen`
- ERVARINGEN → `#video`
- Kennis Maken (CTA button) → `#contact`

### 2. Hero Sectie
**ID:** Geen ID (eerste sectie)
**Locatie:** regels ~220-260

**Elementen:**
- Achtergrond foto met overlay
- Badge: "Ruimte voor cijfers en rust in je werk"
- Hoofdtitle: "Werken bij SUM Accountants"
- Introductietekst
- Twee CTA buttons:
  - "Solliciteer Nu" → `#contact` (wit, primary tekst)
  - "Meer Over Ons" → `#missie` (outline wit)

### 3. Missie Sectie
**ID:** `#missie`
**Locatie:** regels ~266-315

**Content:**
- Titel: "Onze missie: werken met een hoger doel"
- Beschrijving van christelijke identiteit
- 4 Waarden kaarten:
  - Kwaliteit (primary)
  - Integriteit (secondary)
  - Teamwork (accent)
  - Flexibiliteit (primary)

### 4. Jouw Rol Sectie
**ID:** `#rol`
**Locatie:** regels ~321-382

**Elementen:**
- Subtitel: "Zelfstandigheid en vakinhoudelijke Groei"
- Beschrijving van de functie
- "De werkdag" kader met iconen:
  - Start 08:30-09:00 uur
  - Gezamenlijke lunch 12:30 uur
  - Rustige sfeer
  - Klaar rond 17:00 uur

### 5. Antoinette Quote + Video
**ID:** Geen ID
**Locatie:** regels ~384-435

**Layout:** 2 kolommen
- **Links:** Quote over werkdruk + foto
- **Rechts:** 1:1 YouTube video (1 minuut interview)

**Video details:**
- URL: `https://www.youtube.com/embed/8zWu9XJS7nU`
- Formaat: 1:1 (vierkant)
- Badge: "1 minuut met Antoinette"

### 6. De SUM-match Sectie
**ID:** `#match`
**Locatie:** regels ~437-515

**Content:**
- Donkere achtergrond met tekst in wit
- Twee kolommen:
  - **Links (Groen):** "WEL voor jou als" - 5 punten
  - **Rechts (Rood):** "NIET voor jou als" - 4 punten

### 7. Wat Wij Jou Bieden
**ID:** `#voordelen`
**Locatie:** regels ~517-551

**Arbeidsvoorwaarden:**
- Salaris indicatie
- Vakantiegeld
- Pensioen
- Opleidingsmogelijkheden
- Flexibele werktijden
- Gezonde werk-privé balans

### 8. Video Sectie - Medewerkers
**ID:** `#video`
**Locatie:** regels ~553-599

**Video details:**
- URL: `https://www.youtube.com/embed/UE-zvECkBz4`
- Formaat: 16:9 (breed)
- Badge: "Medewerkers aan het woord"
- Quote: "Het voelt niet als werken..."

### 9. Cultuur Sectie
**ID:** Geen ID
**Locatie:** regels ~601-660

**Content:**
- Achtergrond foto (team overleg)
- Links: "Onze cultuur: veiligheid en vertrouwen"
- Rechts: "Jouw weg naar SUM" timeline

**Timeline stappen:**
1. Sollicitatie
2. Kennismaking
3. Meedraaien
4. Aanbod

### 10. FAQ Sectie
**ID:** Geen ID
**Locatie:** regels ~662-700

**Vragen (HTML `<details>` elements):**
1. Hoe ziet de christelijke identiteit eruit op kantoor?
2. Word ik goed begeleid?
3. Zijn er doorgroeimogelijkheden?
4. Kan ik ook parttime werken?
5. Hoe zit het met het salaris?
6. Hoe zit het met de parkeergelegenheid?

### 11. Contact Sectie
**ID:** `#contact`
**Locatie:** regels ~702-722

**Elementen:**
- Achtergrond foto (koffie moment)
- Koffie emoji ☕
- Titel: "Zullen we een kop koffie drinken?"
- CTA button: "Neem contact op" → `/` (root)

### 12. Footer
**Locatie:** regels ~724-728

**Content:**
```
© 2026 SUM accountants. All rights reserved.
Link: https://sumaccountants.nl/
```

### 13. Sticky WhatsApp Button
**Locatie:** regels ~730-744

**Details:**
- Positie: Fixed bottom-right
- Telefoonnummer: `06 50218660` (in URL: `31650218660`)
- Tekst: "Chat met Antoinette over de baan"
- Pre-filled message: "Hoi Antoinette, ik zag de vacature en graag even meer weten"

---

## Contact Gegevens

### Bedrijf
- **Naam:** SUM Accountants
- **Locatie:** Krimpen aan den IJssel
- **Website:** https://sumaccountants.nl/

### Contactpersoon
- **Naam:** Antoinette
- **Functie:** Oprichter
- **Telefoon:** 06 50218660
- **WhatsApp:** `https://wa.me/31650218660`

### WhatsApp Link Format
```
https://wa.me/31650218660?text=Jouw%20bericht%20hier
```
- Gebruik `%20` voor spaties
- Gebruik `%2C` voor komma's

---

## Video Content

### 1:1 Interview Video (Antoinette)
- **URL:** `https://www.youtube.com/watch?v=8zWu9XJS7nU`
- **Embed:** `https://www.youtube.com/embed/8zWu9XJS7nU`
- **Duur:** 1 minuut
- **Formaat:** 1:1 (vierkant)
- **Plaatsing:** Naast quote sectie
- **Badge:** "1 minuut met Antoinette"

### Team Video (Medewerkers)
- **URL:** `https://www.youtube.com/watch?v=UE-zvECkBz4`
- **Embed:** `https://www.youtube.com/embed/UE-zvECkBz4`
- **Duur:** ~2 minuten
- **Formaat:** 16:9 (breed)
- **Plaatsing:** Eigen sectie met ID `#video`
- **Badge:** "Medewerkers aan het woord"

### YouTube Embed Parameters
```
?rel=0&modestbranding=1&controls=1&iv_load_policy=3&disablekb=1
```
- `rel=0` - Geen gerelateerde videos na afspelen
- `modestbranding=1` - Minimaliseer YouTube branding
- `controls=1` - Toon afspeelcontrols
- `iv_load_policy=3` - Verberg annotaties
- `disablekb=1` - Schakel keyboard shortcuts uit

---

## Aanpassingen Maken

### Tekst Aanpassen
Zoek de tekst in `index.html` en vervang deze. De meeste teksten staan in duidelijke secties met comments.

```html
<!-- Voorbeeld: Hero titel aanpassen -->
<h1 class="text-4xl font-extrabold text-white sm:text-5xl lg:text-6xl leading-tight">
   Werken bij SUM Accountants  <!-- ← Wijzig dit -->
</h1>
```

### Kleuren Aanpassen
Pas de CSS variabelen aan in de `<style>` section:

```html
<style>
  :root {
    --primary: #7C3AED;      /* ← Wijzig naar gewenste kleur */
    --secondary: #EC4899;
    --accent: #F2C7DF;
    --text: #1F2937;
  }
</style>
```

### Nieuwe FAQ Toevoegen
Kopieer een bestaande `<details>` block en pas de inhoud aan:

```html
<details class="group rounded-xl border border-gray-200 bg-white p-6 shadow-sm transition-all open:shadow-md">
  <summary class="flex items-center justify-between cursor-pointer text-lg font-bold text-[var(--text)]">
    <!-- Jouw vraag hier -->
    Hoe vraag ik dit aan?
    <span class="ml-4 shrink-0 rounded-full bg-gray-100 p-2 text-[var(--primary)] group-open:bg-[var(--primary)] group-open:text-white transition-colors">
      <svg class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
      </svg>
    </span>
  </summary>
  <p class="mt-4 text-gray-600 leading-relaxed">
    <!-- Jouw antwoord hier -->
    Hier komt het antwoord op de vraag.
  </p>
</details>
```

### Video Vervangen
Vervang de YouTube URL in de `src` attribuut van de `<iframe>`:

```html
<iframe
  src="https://www.youtube.com/embed/JOUW_VIDEO_ID?rel=0&modestbranding=1&controls=1&iv_load_policy=3&disablekb=1"
  <!-- ... overige attributen ... -->
>
```

**YouTube ID vinden:**
- Ga naar de video op YouTube
- De ID is het deel na `v=` in de URL
- Voorbeeld: `https://www.youtube.com/watch?v=UE-zvECkBz4`
- ID is: `UE-zvECkBz4`

### WhatsApp Bericht Aanpassen
Pas de tekst in de WhatsApp link aan (regel ~710):

```html
href="https://wa.me/31650218660?text=Jouw%20nieuwe%20bericht"
```

**URL encoding:**
- Spatie → `%20`
- Komma → `%2C`
- Vraagteken → `%3F`
- En teken → `%26`

### Afbeelding Vervangen
Vervang de `src` van de `<img>` tag:

```html
<img src="images/jouw-nieuwe-foto.jpg" alt="Beschrijving">
```

**Aanbevolen afmetingen:**
- Hero achtergrond: 2048px breed, ~1400px hoog
- Team foto's: 2048px breed, ~1000px hoog
- Profiel foto's: 200x200px (vierkant)

### Link Aanpassen
Zoek de `href` attributen en pas aan:

```html
<a href="https://jouw-website.nl">Tekst</a>
```

---

## Git Geschiedenis

### Recente Commits

| Commit | Datum | Beschrijving |
|--------|-------|--------------|
| `de04a3f` | Jan 2026 | Update WhatsApp button text to 'Chat met Antoinette over de baan' |
| `ce1b142` | Jan 2026 | Move 1:1 video next to existing Antoinette quote section |
| `ee9e80a` | Jan 2026 | Redesign 1:1 video section with 2-column layout and update WhatsApp link |
| `e31297e` | Jan 2026 | Add 1:1 Antoinette interview video and WhatsApp contact button |
| `d00caa3` | Jan 2026 | Add salary FAQ and improve workday section styling |
| `c444458` | Jan 2026 | Add employee interview video section |
| `11c177b` | Jan 2026 | Redesign header with modern sticky navigation |

### Commando's

**Status bekijken:**
```bash
git status
```

**Wijzigingen committen:**
```bash
git add index.html
git commit -m "Beschrijving van wijzigingen"
git push
```

**Vorige versie herstellen:**
```bash
git log --oneline  # Bekijk commits
git checkout [commit-hash]  # Herstel specifieke commit
```

---

## Browser Testing

### Lokale Testing
Gebruik een lokale server om de pagina te testen:

```bash
# Python (meestal aanwezig)
python -m http.server 8000

# Open browser naar:
# http://localhost:8000
```

### Responsive Breakpoints
- **Mobiel:** < 768px (sm)
- **Tablet:** 768px - 1024px (md)
- **Desktop:** > 1024px (lg+)

### Browser Ondersteuning
- ✅ Chrome/Edge (Chromium)
- ✅ Firefox
- ✅ Safari
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

---

## To Do / Toekomstige Verbeteringen

- [ ] SEO meta tags toevoegen
- [ ] Open Graph tags voor social media
- [ ] Google Analytics integratie
- [ ] Sollicitatie formulier toevoegen
- [ ] Meer medewerker video's
- [ ] Accommodatie sectie (kantoor foto's)
- [ ] Blogs/Nieuws sectie?

---

## Support

Vragen of problemen? Neem contact op met de developer of bekijk de Git geschiedenis voor eerdere wijzigingen.

**GitHub:** https://github.com/raket-online/werkenbijsum.git

---

*Dit document is laatst bijgewerkt op 27 januari 2026*
