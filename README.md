# Spatlappen CRM — OAuth-informatiesite

Een openbare, statische informatie-website voor de Google OAuth-branding van Spatlappen CRM. De site staat los van de CRM-applicatie en bevat geen klantgegevens, accounts, formulieren, trackers of toegang tot CRM-dossiers.

## Lokale controle

Open `index.html` direct in een browser of serveer deze map met een lokale HTTP-server. De site gebruikt alleen HTML en CSS.

## GitHub Pages

De links zijn relatief en werken zowel op een rootdomein als onder het repositorypad `/spatlappen-crm-info/`. Schakel na de eerste push in de repository-instellingen GitHub Pages in met branch `main`, map `/` (root). De verwachte URL's:

- Home: <https://website-voorbeelden.github.io/spatlappen-crm-info/>
- Privacy: <https://website-voorbeelden.github.io/spatlappen-crm-info/privacy/>
- Gebruiksvoorwaarden: <https://website-voorbeelden.github.io/spatlappen-crm-info/terms/>
- Support: <https://website-voorbeelden.github.io/spatlappen-crm-info/support/>

Alle HTML-pagina's zetten `noindex`-metatags; er is bewust geen `robots.txt` of sitemap. Dit voorkomt geen directe toegang: Google moet de pagina's kunnen ophalen om de metatags te zien.

## Google OAuth-controle

Google vereist voor merkverificatie een openbare homepage met duidelijke uitleg, plus een openbare privacyverklaring en eventueel voorwaarden. Google kan ook eigendomsverificatie van de domeinen in de OAuth-configuratie verlangen. Een `github.io`-URL kan daarvoor onvoldoende zijn als de OAuth-console domeineigendom van een eigen domein vraagt. Verifieer `spatlappenopmaat.nl` in Search Console met een Google-account dat bij het Cloud-project hoort en gebruik bij voorkeur een eigen subdomein voor de informatiepagina als Google dat vereist.

Google kan aanvullende controle vragen voor gevoelige of beperkte Gmail-scopes. Alleen een informatiesite publiceren garandeert dus niet dat de Gmail-integratie in productie wordt goedgekeurd.

## Eigenaar moet vóór indiening bevestigen

De privacyverklaring markeert expliciet wat niet kon worden geverifieerd in de CRM-code die beschikbaar was voor deze site. Bevestig vóór de OAuth-aanvraag de exacte Gmail-scopes en opgehaalde gegevens, de tokenversleuteling en toegang, bewaartermijnen en verwijdering (ook na intrekking en in back-ups), en de juridische identiteit/adres van de verwerkingsverantwoordelijke. Houd de gepubliceerde verklaring in overeenstemming met de daadwerkelijke productie-implementatie.

## Bronnen

- [Google OAuth brand verification](https://developers.google.com/identity/protocols/oauth2/production-readiness/brand-verification)
- [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy)
- [Google OAuth 2.0 policies](https://developers.google.com/identity/protocols/oauth2/policies)
