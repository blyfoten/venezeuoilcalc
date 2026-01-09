# Venezuelansk olja – ekonomisimulator

En interaktiv ekonomisimulator för att analysera potentiella intäkter och kostnader från Venezuelas oljeproduktion.

[Try It!](https://html-preview.github.io/?url=https://github.com/blyfoten/venezeuoilcalc/raw/refs/heads/main/index.html)

## Funktioner

Simulatorn låter dig justera olika parametrar och se realtidsresultat:

### Produktionsparametrar
- **Produktion**: Antal fat per dag (100k - 3M fat/dag)
- **Marknadspris**: USD per fat ($30-$150)
- **Exportandel**: Andel av produktion som exporteras (0-100%)
- **Sanktionsrabatt**: Rabatt mot spotpris på grund av sanktioner/risk (0-40%)

### Kostnadsparametrar
- **Upstream OPEX**: Lyft- och driftkostnad ($3-$35/fat)
- **Transport**: Transport, försäkring och logistik ($0-$20/fat)
- **Raffinering**: Andel som raffineras, kostnad och marginal
- **CAPEX**: Investeringar och modernisering (årlig kostnad)
- **Infrastruktur**: Extra underhåll och drift (årlig kostnad)
- **Militär närvaro**: Optional kostnad för militär närvaro i Venezuela (årlig kostnad)
- **Förluster**: Förluster genom stöld och ineffektivitet (0-20%)

### Fördelningsparametrar
- **Befolkning**: Andel av nettovinst till befolkningen (%)
- **USA**: Andel av nettovinst till USA (%)
- **Staten**: Andel av nettovinst till venezuelanska staten (%)

## Resultat

Simulatorn visar:
- **KPIs**: Årlig netto till USA och total nettovinst
- **Breakdown**: Detaljerad uppdelning av intäkter och kostnader
- **Fördelning**: Visualisering av hur nettovinsten fördelas (cirkeldiagram)
- **Känslighetsanalys**: Graf som visar hur prisvariationer påverkar resultaten

## URL-delning

Du kan spara och dela dina parametrar genom att kopiera länken med "Kopiera länk med parametrar"-knappen. Alla parametrar sparas i URL:en så att andra kan se samma scenario.

## Antaganden

Modellen använder förenklade antaganden och är till för "what-if"-analyser:
- Exporterade volymer = produktion × exportandel × (1 − förluster)
- Effektivt pris = marknadspris × (1 − rabatt)
- Raffinaderibidrag: (raffinaderimarginal − raffinaderikostnad) × raffinerade fat
- Totalkostnader = upstream OPEX + transport + raffinaderikostnad + CAPEX + infrastruktur + militär närvaro
- Andelar normaliseras om de inte summerar till 100%
