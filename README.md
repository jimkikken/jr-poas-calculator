# JR POAS Calculator

ROAS en POAS calculator voor e-commerce ondernemers. Twee modi:

- **Eenvoudig** — snelle berekening met marge, ad spend en overige kosten.
- **Geavanceerd** — volledige e-commerce berekening met retouren, PSP-fees (vast + procentueel), restock-percentage, retourshipping, LTV multiplier en een winstopbouw-tabel.

## Live

**https://jimkikken.github.io/jr-poas-calculator/**

## Embedden

Gebruik een iframe:

```html
<iframe
  src="https://jimkikken.github.io/jr-poas-calculator/"
  style="width:100%;height:1400px;border:0"
  title="ROAS &amp; POAS Calculator"
  loading="lazy">
</iframe>
```

Pas de hoogte aan naar je pagina. De calculator is responsive en werkt vanaf 320px breed.

## Formules

Zie inline JavaScript in `index.html` voor de exacte berekeningen. Kernpunten:

- **LTV-multiplier** werkt op de contributiemarge (winst vóór ad spend), niet op de netto winst. Herhaalaankopen kosten geen nieuwe advertentie-euro's.
- **PSP transactiekosten** worden berekend op bruto omzet (refunds worden door Mollie/Stripe/Adyen meestal niet terugbetaald) en kennen zowel een procentueel als een vast deel per transactie.
- **Retourshipping** wordt apart berekend, voor het geval jij de retourlabels betaalt.
- **Restock-percentage** modelleert welk deel van geretourneerde voorraad opnieuw verkocht kan worden (fashion 80-90%, consumables 0%).
- **Overige variabele kosten** worden op bruto omzet berekend, omdat pick & pack en verpakking ook voor later geretourneerde orders wordt gedaan.

## Versies

- **1.0.0** — Initial release.

## Licentie

Eigendom van James Robinson B.V. Voor gebruik binnen JR-klantprojecten.
