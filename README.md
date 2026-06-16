# Ooms Media — Premium webdesign studio

De officiële website van **Ooms Media** — een premium, cinematische one-page
ervaring voor een webdesign studio uit Zeeland, Nederland.

Gebouwd als een **volledig statische site** (HTML · CSS · JavaScript) zonder
build-stap: razendsnel, eenvoudig te hosten en zonder afhankelijkheden die
kunnen breken.

> Dark obsidian navy · electric cyan · glassmorphism · cinematische glow ·
> oversized typografie · premium motion.

---

## ✦ Structuur

```
index.html        → de volledige pagina (alle 11 secties)
css/style.css     → design system + alle componenten & secties
js/main.js        → navigatie, reveals, parallax, before/after-slider,
                    interactieve strategie-form (WhatsApp/e-mail)
assets/           → logo's, founder-foto, social share-afbeelding
robots.txt        → SEO
sitemap.xml       → SEO  (pas het domein aan indien nodig)
```

## ✦ Secties

1. **Cinematische hero** — fog gradients, parallax floating UI, oversized titel
2. **Trust** — marquee, kerncijfers, branche-vertrouwen
3. **Diensten** — 6 premium service cards
4. **Werk** — sleepbare voor/na-vergelijking + device-showcase
5. **Waarom Ooms Media** — psychologie van de eerste indruk
6. **Over Juriaan** — oprichter & vertrouwen
7. **Strategie** — interactieve multi-select doelen + premium formulier
8. **Proces** — tijdlijn in 4 stappen
9. **Prijzen** — Starter / Premium / Growth (vanaf-prijzen, eenmalig)
10. **FAQ** — uitklapbare vragen
11. **CTA + Footer** — WhatsApp, contact, system-metadata

## ✦ Lokaal bekijken

Open `index.html` direct in de browser, of start een mini-server:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## ✦ Online zetten

- **GitHub Pages:** Settings → Pages → *Deploy from a branch* → branch `main`,
  map `/ (root)` → Save. Binnen een minuut live.
- **Vercel / Netlify:** importeer de repo. Geen build command nodig
  (statische site, output directory: root).

> Het canonieke domein staat ingesteld op `oomsmedia.nl` (in `index.html`,
> `robots.txt` en `sitemap.xml`). Pas dit aan zodra het definitieve domein
> bekend is.

## ✦ Interactieve strategie-form (met échte e-mail)

In de sectie **Strategie** selecteert de bezoeker doelen; daarna verschijnt een
premium formulier. Bij **Verstuur aanvraag** wordt de aanvraag (inclusief de
gekozen doelen, naam, bedrijf, e-mail, telefoon, huidige website en
opmerkingen) als e-mail verstuurd via **FormSubmit** (`formsubmit.co`) — een
gratis dienst, **geen API-key en geen backend nodig**. Er is daarnaast een
**WhatsApp**-knop die hetzelfde bericht direct in WhatsApp opent.

**Instellen (eenmalig):**

1. Open `js/main.js` en zet bovenaan het juiste adres bij `CONTACT_EMAIL`.
2. Zet de site live (of test lokaal) en verstuur één testaanvraag.
3. Je ontvangt eenmalig een **"Activate Form"**-mail van FormSubmit op dat
   adres → klik die knop één keer. Daarna komt élke aanvraag automatisch binnen.

> De reply-to van elke mail is het e-mailadres van de aanvrager, dus je kunt in
> Gmail direct op de klant antwoorden.

## ✦ Toegankelijkheid & performance

- Semantische HTML, `aria`-labels, focus-states, skip-link
- Volledige `prefers-reduced-motion`-ondersteuning
- Geen frameworks, geen tracking, geen render-blocking JS (`defer`)
- Mobiel-first, getest voor grote touch-targets en soepele motion

## ✦ Contact

Juriaan Ooms · [oomsmedianl@gmail.com](mailto:oomsmedianl@gmail.com) ·
[+31 6 22576578](tel:+31622576578) ·
[WhatsApp](https://wa.me/31622576578) · Zeeland, Nederland
