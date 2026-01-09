# Venezuelan Oil – Economic Simulator

An interactive economic simulator for analyzing potential revenues and costs from Venezuelan oil production.

[Try It!](https://html-preview.github.io/?url=https://github.com/blyfoten/venezeuoilcalc/raw/refs/heads/main/index.html)

## Features

The simulator lets you adjust various parameters and see real-time results:

### Production Parameters
- **Production**: Barrels per day (100k - 3M bbl/day)
- **Market Price**: USD per barrel ($30-$150)
- **Export Share**: Share of production that is exported (0-100%)
- **Sanctions Discount**: Discount against spot price due to sanctions/risk (0-40%)

### Cost Parameters
- **Upstream OPEX**: Lifting and operating cost ($3-$35/bbl)
- **Transport**: Transportation, insurance and logistics ($0-$20/bbl)
- **Refining**: Share that is refined, cost and margin
- **CAPEX**: Investment and modernization (annual cost)
- **Infrastructure**: Extra maintenance and operations (annual cost)
- **Military Presence**: Optional cost for military presence in Venezuela (annual cost)
- **Losses**: Losses through theft and inefficiency (0-20%)

### Distribution Parameters
- **Population**: Share of net profit to the population (%)
- **USA**: Share of net profit to USA (%)
- **State**: Share of net profit to Venezuelan state (%)

## Results

The simulator displays:
- **KPIs**: Annual net to USA and total net profit
- **Breakdown**: Detailed breakdown of revenues and costs
- **Distribution**: Visualization of how net profit is distributed (pie chart)
- **Sensitivity Analysis**: Graph showing how price variations affect results

## URL Sharing

You can save and share your parameters by copying the link with the "Copy link with parameters" button. All parameters are saved in the URL so others can see the same scenario.

## Assumptions

The model uses simplified assumptions and is intended for "what-if" analyses:
- Exported volumes = production × export share × (1 − losses)
- Effective price = market price × (1 − discount)
- Refining contribution: (refining margin − refining cost) × refined barrels
- Total costs = upstream OPEX + transport + refining cost + CAPEX + infrastructure + military presence
- Shares are normalized if they don't sum to 100%
