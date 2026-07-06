# Rihlaturruh — website

Een premium, fotografisch geïnspireerde website met tabbladen, opgebouwd als **één bestand** (`index.html`). Gratis te testen via **GitHub Pages**.

Tabbladen: **Home · Over mij · Diensten & Aanbod · Materialen · Contact** + knop **Plan een consult**.
Onderaan elke pagina: monochrome social-icons (Instagram, TikTok, YouTube, e-mail) passend bij de stijl.
Merkbelofte in de teksten: **Authentiek · Diepgaand · Toepasbaar**.

## Wat zit erin — ALLES uploaden naar GitHub
Upload deze bestanden (in de hoofdmap van de repo):
- `index.html` — de hele website
- `logo.png` — nieuw logo (volledig, deel-afbeelding)
- `logo-mark.png` — ronde logo-versie (header, footer, favicon)
- De 10 foto's:
  - `p-home-hero.jpg`, `p-home-reflect.jpg`, `p-home-visie.jpg` (Home)
  - `p-over-intro.jpg`, `p-over-wie.jpg`, `p-over-achter.jpg` (Over mij)
  - `p-diensten.jpg` (Diensten & Aanbod)
  - `p-materialen.jpg` (Materialen)
  - `p-contact.jpg`, `p-samenwerken.jpg` (Contact)

Alle foto's zijn geoptimaliseerd voor snelle laadtijd. Wil je een foto vervangen? Upload een nieuwe met dezelfde bestandsnaam.

## Bewust nog NIET op de site (gericht op focus)
Volgens je 90-dagenplan bouw je eerst een sterk fundament. Daarom:
- **Geen winkel/Producten-tab.** De reflectiekaartenset is Prioriteit 3 (nog in ontwikkeling). Op de homepagina staat alleen een zachte teaser ("Inschrijvers horen als eerste wanneer de reflectiekaarten verschijnen") die je nieuwsbrieflijst voedt.
- **Nieuwsbrief "Brief aan de Ziel"** staat centraal op Home én Reflecties — zo bouw je je lijst op.

## Online zetten via GitHub Pages (zonder commando's)
1. Account op [github.com](https://github.com).
2. **+** → **New repository** → naam `rihlaturruh` → **Public** → **Create repository**.
3. **uploading an existing file** → sleep `index.html` én `logo.png` erin → **Commit changes**.
4. **Settings** → **Pages** → branch **main**, map **/(root)** → **Save**.
5. Na ~1 minuut: `https://JOUW-NAAM.github.io/rihlaturruh/`

## Tekst aanpassen
Open `index.html` (op GitHub: bestand → potloodje ✏️). Elke sectie staat tussen duidelijke kommentaarregels, bijv. `<!-- ===== OVER MIJ ===== -->`. Let op de tips in het bestand, o.a.:
- "Over mij" — opgesteld vanuit je briefing; maak het je eigen.
- FAQ "Wat kost een consult?" — vul je tarieven/werkwijze in.
- Reflecties — vervang de drie voorbeeldartikelen door je eigen teksten.

## Boekingssysteem — Cal.com (gekoppeld)
De knop **"Boek je consult"** op de Consulten-pagina is gekoppeld aan **`https://cal.eu/rihlaturruh`** (EU-profiel).
- Verandert je adres ooit? Geef het door, dan pas ik de link in één regel aan (zoek in `index.html` op `cal.eu/rihlaturruh`).
- Hernoem je standaard-afspraaktypes naar bv. Kennismaking, Consult en Traject en koppel je agenda. De knop wijst naar je algemene boekingspagina, dus die blijft werken ook als de afspraaknamen veranderen.
- De "Boek een consult"-knoppen op Home en Over mij leiden eerst naar de Consulten-pagina (eerst uitleg, dan boeken).

## Nieuwsbrief — Kit (gekoppeld)
De knoppen **"Schrijf je in"** (Home en Reflecties) en de link op de Contact-pagina wijzen naar je Kit-inschrijfpagina: **`https://brief-aan-de-ziel.kit.com/955c0af13d`**. Inschrijvingen komen automatisch in je Kit-lijst ("Brief aan de Ziel").
- Wil je het formulier later volledig ín je eigen site (zodat mensen niet doorklikken naar Kit)? Kopieer in Kit de **HTML/JavaScript-embedcode** van het formulier en geef die door, dan bouw ik 'm op je eigen pagina in.

## Contactformulier rechtstreeks in je inbox (optioneel, later)
GitHub Pages heeft geen server, dus het contactformulier opent nu je e-mailprogramma. Wil je dat berichten direct in je inbox binnenkomen → **Formspree** (gratis). Zeg het maar, dan bouw ik het in.

## Later uitbreiden (na het fundament)
Wil je in een latere fase tabs toevoegen (Voor professionals · Voor vrouwen · Voor kinderen · Sport & Ziel)? Per tab twee dingen:
1. **Menuknop** in `<nav class="nav">` én `<nav class="mobile-menu">`:
   `<button data-go="vrouwen">Voor vrouwen</button>`
2. **Sectie** onderaan in `<main>`:
   ```html
   <section id="vrouwen" class="page">
     <section class="block"><div class="wrap">
       <p class="eyebrow">Voor vrouwen</p>
       <h2 class="title">Titel</h2>
       <p class="lede">Inleiding…</p>
     </div></section>
   </section>
   ```
   De `id` van de sectie = de `data-go` van de knop.

## Eigen domein (optioneel)
Heb je `rihlaturruh.nl`? Koppelen onder **Settings → Pages → Custom domain**.
