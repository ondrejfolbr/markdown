# 03 WEB & LANDING PAGE (ant)
## Struktura LP (Blueprint)
1. **Hero Sekce:** Jasný claim, (WOW) vizuál, primární CTA.
2. **Problém/Pain Point:** Co klienta pálí?
3. **Řešení (ant) cestou:** Jak to vyřešíme jinak?
4. **Social Proof:** Loga klientů, metriky, výsledky.
5. **Proces:** Jak probíhá spolupráce.
6. **Závěrečné CTA:** "Pojďme se pobavit".

## Vizuální pravidla pro web
- Práce s prostorem (white space).
- Čistá typografie, zarovnání na střed nebo vlevo (nikdy do bloku).
- Interaktivní prvky v Primary Green.

## Typografie pro web
- **Aktiv Grotesk Ex** se na webu načítá přes Adobe Fonts (Typekit), ne z lokálních `.otf`.
- **Embed kód do `<head>`:**
  ```html
  <link rel="stylesheet" href="https://use.typekit.net/zch7ids.css">
  ```
- **Inter** se načítá z Google Fonts (nebo si hostuj `./Inter/static/Inter_18pt-Light.ttf` a `Inter_28pt-Bold.ttf` lokálně, pokud potřebuješ kontrolu nad optickými velikostmi).
- **Font stack v CSS:**
  ```css
  --font-display: "aktiv-grotesk-extended", system-ui, sans-serif;
  --font-body: "Inter", system-ui, sans-serif;
  ```
- **Pravidlo PDF/email:** Pokud generuješ PDF nebo HTML email z webové šablony, font musí být embedded nebo nahrazený fallbackem — Typekit v Outlooku a v izolovaných PDF rendererech nefunguje.