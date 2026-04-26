# website

Codul sursă al site-ului de prezentare [signalforall.ro](https://signalforall.ro).

Single-page HTML cu CSS inline, fără dependențe externe (în afară de Google Fonts pentru tipografie).

## Structură

- `index.html` — fișierul unic care conține întreg site-ul

## Tehnologii

- HTML5 semantic
- CSS3 (custom properties, grid, flexbox, animations)
- Google Fonts: Fraunces (display serif), Inter Tight (sans), JetBrains Mono (mono)
- IntersectionObserver pentru reveal animations la scroll

Site-ul este conceput să funcționeze fără JavaScript pentru conținutul de bază — animațiile sunt progressive enhancement.

## Accesibilitate

- Semantică HTML corectă (header, nav, section, article, footer)
- Atribute ARIA unde e cazul
- Focus styles vizibile pentru navigare keyboard
- Suport pentru `prefers-reduced-motion`
- Contrast verificat (paleta forest/cream/ochre îndeplinește WCAG AA)

## Cum se rulează local

Fișierul `index.html` este self-contained. Poate fi:
1. Deschis direct în browser (`Ctrl+O` → selectează `index.html`)
2. Servit cu orice server HTTP simplu:

```bash
# Cu Python
python3 -m http.server 8000

# Cu Node.js (npx)
npx serve

# Cu PHP
php -S localhost:8000
```

Apoi navighezi la `http://localhost:8000`.

## Deploy

Site-ul live pe [signalforall.ro](https://signalforall.ro) este găzduit pe shared hosting (cPanel) cu fișierul `index.html` în `public_html/`.

## Versiuni

- **v1.0** — versiunea inițială (4 secțiuni: Problema, Cum funcționează, Parcurs, Despre)
- **v1.1** — adăugat secțiunea "Status actual" + icoane SVG la fluxul Cum funcționează
- **v1.2** — adăugat nota clarificatoare în footer despre signalforall.com

## Licență

Cod: GPL-3.0  
Conținut text și imagini: CC BY-SA 4.0

## Contribuții

Pull request-uri și issue-uri sunt binevenite. Pentru schimbări mari, deschide un issue pentru discuție înainte.
