# Tradecraft: recorded demo data

Data for the keyless demo of Tradecraft. Clone this repository into the main
repository's `data/demo-bundle/` folder, then follow "Recorded demo" in the main
README. It lets all four stages be clicked through with no API key, no network
and no cost.

Everything here is a recording made on 19 November 2026. It is not live data and not
investment advice. Tradecraft places no orders.

| Folder | What it is | Source |
|---|---|---|
| `snapshot/` | One option-chain snapshot, cut down to AMZN, MSFT, NVDA | Cboe delayed quotes, as logged by the project's daily job |
| `prices/` | Daily closing prices for the same symbols | Yahoo chart endpoint |
| `stage2/` | What the thesis stage's agents returned on a real run, with the evidence they cited | SEC EDGAR filings, Financial Modeling Prep, the Federal Reserve and FRED calendars; model output from Claude |
| `stage4/` | What the Evidence Retriever and the Critic returned on a real run, per selected strategy | The project's own research; model output from Claude |
| `events.json`, `symbols.json`, `manifest.json` | Dividend dates, the symbol list for the search box, the date of the data | Financial Modeling Prep; public listing files |

The third-party data is a small sample kept so that the software can be evaluated.
It is not licensed for reuse; take it from its source if you need it.
