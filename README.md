# Bazzar Dental Office

Statični sajt ordinacije. Nema build koraka — svi fajlovi se serviraju kako jesu.

## Hostovanje na GitHub Pages

1. Napravite repozitorijum i ubacite sadržaj ove `site/` fascikle u koren repozitorijuma.
2. Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. Sačekajte minut; sajt je na `https://korisnik.github.io/ime-repozitorijuma/`.

Fajl `.nojekyll` je dodatna sigurnost, ali nije neophodan — nijedna fascikla ne počinje podvlakom.

## Struktura

- `index.html` — cela stranica
- `support.js` — runtime
- `image-slot.js` — polja za slike
- `ds/` — stilovi dizajn sistema

## Slike

Polja za slike su prazna. Slike ubačene prevlačenjem u editoru se ne prenose u ovaj export — u `index.html` zamenite `<image-slot ...></image-slot>` običnim `<img src="slike/ime.jpg" style="width:100%;height:100%;object-fit:cover">` i ubacite fajlove u fasciklu `slike/`.

## Booking

Kalendar je trenutno prototip — zahtevi se nigde ne šalju. Za pravo zakazivanje: Cal.com link se upisuje u `calLink()` funkciju u `index.html`.
