# Projekti
Henkilökohtainen portfoliosivusto. Pelkkä index.html + style.css, ei build-työkaluja, ei JS-kehyksiä.

# Rakenne
- index.html — kaikki sisältö, data-fi/data-en -attribuutit kaksikielisyyteen (toggleLang())
- style.css — 9 CSS-muuttujaa :root:ssa (--bg, --bg2, --bg3, --accent, --text, --text-dim, --white, --border, --green), vaalea teema override html[data-theme="light"]:ssa
- sertifikaatit/ — PDF-sertifikaatit, linkitetty Taidot-osion "AI-työkalut"-alaotsikon alle (ei "Ohjelmointitaidot"-osioon)

# Konventiot
- Uusi teksti-sisältö tarvitsee aina sekä data-fi että data-en -attribuutin
- Väreissä käytä aina olemassa olevia CSS-muuttujia, älä hardkoodaa uusia
- Ei build/testi-työkaluja — verifiointi aina paikallisen HTTP-palvelimen kautta (ei file://) ja Claude in Chromella

# Git-workflow
- Commitoidaan suoraan main-branchiin, ei PR-työnkulkua

# Muistettavaa (ei toisteta enää)
- ÄLÄ ehdota AI-diligence-/avoimuuslausunnon lisäämistä sivustolle. Käyttäjä on nimenomaisesti kieltäytynyt tästä henkilökohtaisella portfoliollaan, tietoisena päätöksenä.
