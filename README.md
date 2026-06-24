# Rihlaturruh — website

Een website met tabbladen, opgebouwd als **één bestand** (`index.html`). Je test 'm gratis online via **GitHub Pages**.

Tabbladen nu: **Home · Over · Consulten · Reflecties · Producten · Contact**
Onderaan elke pagina: social-icons voor Instagram, TikTok, YouTube en e-mail.

## Wat zit erin
- `index.html` — de hele website (menu, alle tabbladen, formulieren)
- `logo.png` — je logo (ook favicon + deel-afbeelding)

## Online zetten via GitHub Pages (zonder commando's)
1. Account op [github.com](https://github.com).
2. Rechtsboven **+** → **New repository** → naam `rihlaturruh` → **Public** → **Create repository**.
3. Klik **uploading an existing file** en sleep `index.html` én `logo.png` erin → **Commit changes**.
4. **Settings** → **Pages** → branch **main**, map **/(root)** → **Save**.
5. Na ~1 minuut verschijnt je link: `https://JOUW-NAAM.github.io/rihlaturruh/`

## Hoe de tabbladen werken
Alles staat op één pagina; het menu wisselt tussen secties (#home, #over, …). Je kunt dus rechtstreeks naar een tab linken, bijv. `.../rihlaturruh/#consulten`.

## Tekst aanpassen
Open `index.html` (op GitHub: bestand openen → potloodje ✏️). Elke sectie staat tussen duidelijke kommentaarregels, bijv. `<!-- ======= OVER ======= -->`. De "Over"-tekst is opgesteld vanuit je briefing — pas 'm gerust aan naar je eigen woorden.

## Extra tabbladen later toevoegen (Professionals · Vrouwen · Kinderen · Sport & Ziel)
Per nieuwe tab twee dingen:
1. **Menuknop** — voeg in `<nav class="nav">` én in `<nav class="mobile-menu">` toe:
   `<button data-go="vrouwen">Voor vrouwen</button>`
2. **Sectie** — voeg onderaan in `<main>` toe:
   ```html
   <section id="vrouwen" class="page">
     <section class="block"><div class="wrap">
       <p class="eyebrow">Voor vrouwen</p>
       <h2 class="title">Titel</h2>
       <p class="lede">Inleiding…</p>
     </div></section>
   </section>
   ```
   De `id` van de sectie moet exact gelijk zijn aan de `data-go` van de knop.

## Let op: boekingen & formulieren
GitHub Pages serveert alleen "statische" bestanden — er draait geen server. Daarom:
- **Consult aanvragen / contactformulier / nieuwsbrief** openen nu je e-mailprogramma met een vooraf ingevuld bericht naar rihlaturruh@gmail.com. Dat werkt direct, zonder kosten.
- Wil je een **echt boekingssysteem** (agenda met tijdslots)? Koppel later een gratis dienst zoals **Cal.com** of **Calendly**: zet de link op de knop "Consult aanvragen".
- Wil je een **echt contactformulier** dat in je inbox binnenkomt (zonder mailprogramma)? Gebruik bijv. **Formspree** (gratis); ik help je dat inbouwen.

## Eigen domein (optioneel)
Heb je bijv. `rihlaturruh.nl`? Koppelen kan onder **Settings → Pages → Custom domain**.
