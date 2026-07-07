---
name: pre-commit-review
description: Tarkistaa muutokset ennen committia tälle portfoliosivustolle. Käytä kun ollaan committaamassa, pushaamassa tai kun käyttäjä pyytää koodikatselmointia.
---

Kun tarkistat muutoksia ennen committia:

1. Aja tuore subagent joka lukee git diffin riippumattomasti (ei saa muokata tiedostoja, vain read-only-työkalut).
2. Tarkista erityisesti:
   - Käytetäänkö olemassa olevia CSS-muuttujia (--bg, --bg2, --bg3, --accent, --text, --text-dim, --white, --border, --green) hardkoodattujen värien sijaan
   - Onko uudella tekstisisällöllä sekä data-fi että data-en -attribuutit
   - Ei oleteta build- tai testityökaluja - verifiointi pitää tehdä paikallisen HTTP-palvelimen kautta (ei file://) ja mielellään Claude in Chromella
3. Anna verdict (Approve/muutoksia tarvitaan) ja yhteenveto löydöksistä ennen kuin committia tehdään.
