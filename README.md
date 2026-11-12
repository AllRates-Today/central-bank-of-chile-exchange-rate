# Central Bank of Chile Exchange Rates API — central-bank-of-chile-exchange-rate

[![npm version](https://img.shields.io/npm/v/central-bank-of-chile-exchange-rate.svg)](https://www.npmjs.com/package/central-bank-of-chile-exchange-rate)
[![license](https://img.shields.io/npm/l/central-bank-of-chile-exchange-rate.svg)](https://github.com/AllRates-Today/central-bank-of-chile-exchange-rate/blob/main/LICENSE)
[![zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://www.npmjs.com/package/central-bank-of-chile-exchange-rate)
[![TypeScript](https://img.shields.io/badge/TypeScript-types%20included-3178C6.svg)](https://www.typescriptlang.org/)
[![USD/CLP today](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fbcch%3Fsource%3DUSD%26target%3DCLP&query=%24.rate&label=USD%2FCLP%20official%2C%20Central%20Bank%20of%20Chile&color=0A7E8C&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/bcch/)
[![rate date](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fbcch%3Fsource%3DUSD%26target%3DCLP&query=%24.rate_date&label=rate%20date&color=555&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/bcch/)

**Official Central Bank of Chile (Chile) daily exchange rates for Node.js and TypeScript. The published central bank rates behind tax filings, customs valuations, audits, and compliant invoicing — not market estimates, but the numbers Central Bank of Chile itself prints, every business day.**

## 🚀 Why this client?

- 🏛️ **Official rates** — Central Bank of Chile's own table, with the publisher's own `rate_date` on every response
- 📅 **History back to 1982** — point-in-time tables and daily series for any past date
- 🔀 **Official vs derived, always flagged** — computed inverse/cross pairs carry `derived: true`, never mixed with official prints
- ⚡ **Zero dependencies** — pure ESM + CJS over global `fetch`; Node 18+, Bun, Deno, and edge runtimes
- 🔷 **Type-safe** — full TypeScript definitions shipped with the package
- 🧾 **Compliance-grade metadata** — `rate_type`, publication date, and source disclaimer on every response

> **Official rate, not mid-market:** every value here is a number Central Bank of Chile itself published, fixed once printed and carrying the central bank's own `rate_date` — what filings and audits require. Need the live mid-market rate for pricing or display instead? Use the [mid-market API](https://allratestoday.com/docs/) or [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk). The two can diverge by several percent.

## 🔑 Get your API key

Get a free API key at [allratestoday.com/register](https://allratestoday.com/register) — no credit card required. Latest rates are on every plan, including free.

## 📈 Latest official table

[![Latest Central Bank of Chile table](https://allratestoday.com/api/open/central-bank/bcch/table.svg)](https://allratestoday.com/central-bank-rates-api/bcch/)

The image is rendered live from the keyless endpoint, so it follows the central bank's publications on npm and on GitHub alike without a new release. The same table as text is folded below for search and copy-paste: on GitHub [a daily Action](.github/workflows/daily-table.yml) refreshes it whenever the central bank publishes a new table; on npm it is as of the package's publish date.

<!-- daily-table:start -->
<details>
<summary>Table as text: published 2026-11-12 by Central Bank of Chile — 60 rates. Updated 2026-11-12.</summary>

| Base | Quote | Type | Rate |
| --- | --- | --- | ---: |
| USD | AED | reference | 3.672 |
| USD | ARS | reference | 1545.3974 |
| USD | AUD | reference | 1.4599 |
| USD | BMD | reference | 1 |
| USD | BOB | reference | 11.71 |
| USD | BRL | reference | 5.5617 |
| USD | BSD | reference | 1 |
| USD | CAD | reference | 1.4248 |
| USD | CHF | reference | 0.8334 |
| USD | CLP | reference | 984.49 |
| USD | CNY | reference | 6.6737 |
| USD | COP | reference | 3281.5533 |
| USD | CRC | reference | 446.16 |
| USD | CUP | reference | 24 |
| USD | CZK | reference | 21.9836 |
| USD | DKK | reference | 6.7401 |
| USD | DOP | reference | 60.348 |
| USD | EGP | reference | 53.5092 |
| USD | EUR | reference | 0.9017 |
| USD | FJD | reference | 2.2769 |
| USD | GBP | reference | 0.7533 |
| USD | GTQ | reference | 7.6365 |
| USD | HKD | reference | 7.8448 |
| USD | HUF | reference | 328.9417 |
| USD | IDR | reference | 18144 |
| USD | ILS | reference | 3.1737 |
| USD | INR | reference | 93.6875 |
| USD | IRR | reference | 1909436 |
| USD | ISK | reference | 122.9967 |
| USD | JPY | reference | 159.8733 |
| USD | KRW | reference | 1336.23 |
| USD | KYD | reference | 0.82 |
| USD | KZT | reference | 445.07 |
| USD | MAD | reference | 9.8071 |
| USD | MXN | reference | 18.6157 |
| USD | MYR | reference | 4.071 |
| USD | NOK | reference | 9.5532 |
| USD | NZD | reference | 1.7975 |
| USD | PAB | reference | 1 |
| USD | PEN | reference | 3.4084 |
| USD | PHP | reference | 63.24 |
| USD | PKR | reference | 276.4761 |
| USD | PLN | reference | 3.9799 |
| USD | PYG | reference | 6202 |
| USD | QAR | reference | 3.6451 |
| USD | RON | reference | 4.8182 |
| USD | RUB | reference | 82.3375 |
| USD | SAR | reference | 3.75 |
| USD | SEK | reference | 9.983 |
| USD | SGD | reference | 1.2849 |
| USD | THB | reference | 33.7672 |
| USD | TRY | reference | 50.2288 |
| USD | TWD | reference | 32.855 |
| USD | UAH | reference | 45.3222 |
| USD | UYU | reference | 40.462 |
| USD | VES | reference | 899.3635 |
| USD | VND | reference | 25640.3333 |
| USD | XDR | reference | 0.74 |
| USD | XPF | reference | 105.8093 |
| USD | ZAR | reference | 16.5945 |

</details>

Source: [Official rates published by BCCH, served by AllRatesToday](https://allratestoday.com/central-bank-rates-api/bcch/). Rates are as printed by the central bank; AllRatesToday is not affiliated with it.
<!-- daily-table:end -->

## 📦 Installation

```bash
npm install central-bank-of-chile-exchange-rate
```

```bash
yarn add central-bank-of-chile-exchange-rate
```

```bash
pnpm add central-bank-of-chile-exchange-rate
```

Requires Node 18+ (global `fetch`); also runs on Bun, Deno and edge runtimes. Also published under the org scope as [`@allratestoday/central-bank-of-chile-exchange-rate`](https://www.npmjs.com/package/@allratestoday/central-bank-of-chile-exchange-rate) — same code, same versions.

## 🏁 Quick start

```js
import { getRate } from 'central-bank-of-chile-exchange-rate';

const pair = await getRate('USD', 'CLP', { apiKey: 'art_live_...' });
console.log(pair.rate, pair.rate_date); // the official Central Bank of Chile rate, on the central bank's own date
```

## 📚 API reference

- [Latest pair rate](#latest-pair-rate) — one pair from the latest official table
- [Full official table](#full-official-table) — everything the central bank printed, in one call
- [Table for a date](#table-for-a-date) — the official table for an invoice or filing date
- [Daily time series](#daily-time-series) — one pair across a date range

---

### Latest pair rate

Free plan and up. Pairs the central bank does not print directly are resolved from its table and flagged (see *Official vs derived rates* below).

```js
const pair = await getRate('USD', 'CLP', { apiKey: 'art_live_...' });
```

**Response:**

```javascript
{
  bank: 'bcch',
  name: 'Central Bank of Chile',
  rate_date: '2026-11-11',   // Central Bank of Chile's own publication date
  source: 'USD',
  target: 'CLP',
  rate: 977.05,
  rate_type: 'reference',
  derived: false,
  method: 'published',
  disclaimer: 'Official rates as published by the named central bank. On weekends/holidays the most recent published rate_date is returned.'
}
```

### Full official table

Free plan and up. The complete table for the latest publication date.

```js
import { getLatestRates } from 'central-bank-of-chile-exchange-rate';

const table = await getLatestRates({ apiKey: 'art_live_...' });
console.log(table.rate_date, table.rates.length);
```

**Response:**

```javascript
{
  bank: 'bcch',
  name: 'Central Bank of Chile',
  rate_date: '2026-11-11',
  rates: [
    { "base": "USD", "quote": "CLP", "type": "reference", "value": 977.05 },
    // … the rest of the official table (60 currencies vs CLP)
  ],
  disclaimer: '…'
}
```

### Table for a date

Paid plans. The official table for any date since 1982 — weekends and holidays return the most recent published date, flagged via `published_on_requested_date`, which is exactly the in-force rate a filing needs.

```js
import { getRatesForDate } from 'central-bank-of-chile-exchange-rate';

const day = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...' });
// Optionally narrow to one pair:
const one = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...', source: 'USD', target: 'CLP' });
```

**Response:**

```javascript
{
  bank: 'bcch',
  requested_date: '2026-06-30',
  rate_date: '2026-06-30',                // the date actually published
  published_on_requested_date: true,      // false when a weekend/holiday fell back
  rates: [ /* the full table for that date */ ],
  disclaimer: '…'
}
```

### Daily time series

Paid plans. One resolved rate per publication date — ready for charting, revaluation runs, or audit workpapers.

```js
import { getHistory } from 'central-bank-of-chile-exchange-rate';

const series = await getHistory(
  { source: 'USD', target: 'CLP', from: '2026-01-01', to: '2026-11-11' },
  { apiKey: 'art_live_...' }
);
```

**Response:**

```javascript
{
  bank: 'bcch',
  source: 'USD',
  target: 'CLP',
  from: '2026-01-01',
  to: '2026-11-11',
  count: 152,
  rates: [
    // one entry per publication date
    { date: '2026-11-11', rate: 977.05, rate_type: 'reference', derived: false, method: 'published' },
    // …
  ],
  disclaimer: '…'
}
```

Pass `{ symbol: 'USD' }` instead of `source`/`target` to get the raw published rows for one currency (all rate types, no pair resolution).

---

## 🗺️ Currencies covered

Central Bank of Chile currently publishes rates covering **60 currencies** against the CLP (as of the latest table):

🇦🇪 `AED` · 🇦🇷 `ARS` · 🇦🇺 `AUD` · 🇧🇲 `BMD` · 🇧🇴 `BOB` · 🇧🇷 `BRL` · 🇧🇸 `BSD` · 🇨🇦 `CAD` · 🇨🇭 `CHF` · 🇨🇳 `CNY` · 🇨🇴 `COP` · 🇨🇷 `CRC` · 🇨🇺 `CUP` · 🇨🇿 `CZK` · 🇩🇰 `DKK` · 🇩🇴 `DOP` · 🇪🇬 `EGP` · 🇪🇺 `EUR` · 🇫🇯 `FJD` · 🇬🇧 `GBP` · 🇬🇹 `GTQ` · 🇭🇰 `HKD` · 🇭🇺 `HUF` · 🇮🇩 `IDR` · 🇮🇱 `ILS` · 🇮🇳 `INR` · 🇮🇷 `IRR` · 🇮🇸 `ISK` · 🇯🇵 `JPY` · 🇰🇷 `KRW` · 🇰🇾 `KYD` · 🇰🇿 `KZT` · 🇲🇦 `MAD` · 🇲🇽 `MXN` · 🇲🇾 `MYR` · 🇳🇴 `NOK` · 🇳🇿 `NZD` · 🇵🇦 `PAB` · 🇵🇪 `PEN` · 🇵🇭 `PHP` · 🇵🇰 `PKR` · 🇵🇱 `PLN` · 🇵🇾 `PYG` · 🇶🇦 `QAR` · 🇷🇴 `RON` · 🇷🇺 `RUB` · 🇸🇦 `SAR` · 🇸🇪 `SEK` · 🇸🇬 `SGD` · 🇹🇭 `THB` · 🇹🇷 `TRY` · 🇹🇼 `TWD` · 🇺🇦 `UAH` · 🇺🇸 `USD` · 🇺🇾 `UYU` · 🇻🇪 `VES` · 🇻🇳 `VND` · `XDR` · `XPF` · 🇿🇦 `ZAR`

## 🏛️ Source

The Central Bank of Chile publishes the dólar observado — the official USD/CLP rate Chilean law, tax and contracts reference, computed from the previous day's interbank trading and published one business day ahead — alongside a parities table of roughly 60 currencies against the dollar. The observado series reaches back to 1982.

- Publisher's own page: [Dólar observado](https://si3.bcentral.cl/Siete/ES/Siete/Cuadro/CAP_TIPO_CAMBIO/MN_TIPO_CAMBIO4/DOLAR_OBS_ADO) · [www.bcentral.cl/en/web/banco-central](https://www.bcentral.cl/en/web/banco-central)
- Publication: every business day; the exact schedule, freshness status and any current delay are on the [Central Bank of Chile rates page](https://allratestoday.com/central-bank-rates-api/bcch/)
- In the API: usually by **21:15 UTC** (measured over the last 11 publications). Schedule a sync at or after that time and retry hourly until `rate_date` moves; every response carries the same figure as `available_by_utc` — see [when to poll](https://allratestoday.com/docs/#when-to-poll)
- Values are stored unmodified, with the publisher's own `rate_date` on every row — see the [methodology](https://allratestoday.com/official-rates-methodology/)

## 🧭 Reading the numbers

- `value` is always **quote currency per 1 unit of base currency** (`base: "EUR", quote: "USD", value: 1.15` means 1 EUR = 1.15 USD).
- Central Bank of Chile quotes **CLP per 1 unit of foreign currency** (e.g. `base: "USD", quote: "CLP"` means CLP per one US dollar).
- Need the other way round? Ask `getRate(target, source)` and the API inverts or crosses for you, flagged `derived: true` — never divide a published rate yourself in a compliance workflow.
- `rate_type` tells you which of the central bank's series a row belongs to (`reference` here); some publishers print buy/sell or several fixings for the same pair.

## 🧩 ERP & accounting systems

Loading the official Central Bank of Chile rate into an accounting system is a supported workflow, not a hack. Step-by-step guides with the direction each system expects:

- [Dynamics 365 Business Central](https://allratestoday.com/docs/integrations/business-central/) — built-in Currency Exchange Rate Service, no code
- [Xero](https://allratestoday.com/docs/integrations/xero/) · [QuickBooks Online](https://allratestoday.com/docs/integrations/quickbooks/) · [SAP S/4HANA and ECC](https://allratestoday.com/docs/integrations/sap/) · [Odoo](https://allratestoday.com/docs/integrations/odoo/)

The same keyed endpoints return `?format=csv`, `?format=xml` and `?format=xlsx`, and accept the key as `?api_key=` on the URL for importers that cannot send headers:

```bash
curl "https://allratestoday.com/api/v1/central-bank/bcch/latest?format=xml&api_key=art_live_..."
```

## 🤖 AI agents

- MCP server: `npx -y @allratestoday/central-bank-mcp` (stdio) or the hosted endpoint `https://allratestoday.com/api/mcp` — tools for official rates, history, cross-bank comparison and publication calendars
- Already using the general SDK or MCP server? Since 2026-10-01 [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk) 1.4+ has `officialRates('bcch')` and [`@allratestoday/mcp-server`](https://www.npmjs.com/package/@allratestoday/mcp-server) 0.6+ has a `get_official_rates` tool — both return this source's latest table with no key, so you can add it without a second dependency
- Claude Code plugin (no key): `/plugin marketplace add AllRates-Today/claude-code-plugin` then `/plugin install allratestoday@allratestoday` — bundles both MCP servers plus an `/official-rate bcch ...` command
- Evaluating? Agents can self-issue a trial key with no signup: `POST https://allratestoday.com/api/agent/keys` (send `Content-Type: application/json`) returns a 100-call key valid 7 days that covers the free-plan methods (latest table, pairs); dated tables and history need a [paid plan](https://allratestoday.com/pricing/). The MCP servers expose it as `request_trial_key`
- Machine-readable site guide: [llms.txt](https://allratestoday.com/llms.txt) · [for-ai-agents](https://allratestoday.com/for-ai-agents/)

## ⚖️ Official vs derived rates

If Central Bank of Chile does not print a pair directly, the API resolves it from the central bank's own table and says so — official and computed values are never confused:

| `method` | `derived` | Meaning |
| --- | --- | --- |
| `published` | `false` | The central bank printed this pair directly |
| `inverse` | `true` | Computed as 1 ÷ the published opposite direction |
| `cross` | `true` | Computed via CLP from two published rates |

## 🛡️ Error handling

Errors are thrown as `Error` with `status` (HTTP code) and `body` (the API's JSON error) attached:

```js
try {
  const pair = await getRate('USD', 'XXX', { apiKey: 'art_live_...' });
} catch (err) {
  console.log(err.message); // human-readable reason
  console.log(err.status);  // e.g. 404
}
```

| Status | Meaning |
| ------ | ------- |
| — | Missing `apiKey` (thrown before any request) |
| `400` | Malformed date or parameters |
| `401` | Invalid API key |
| `403` | Endpoint needs a [paid plan](https://allratestoday.com/pricing/) (historical dates & series) |
| `404` | Pair or date range not covered by Central Bank of Chile |
| `429` | Monthly quota exceeded |

## 🔷 TypeScript

Full definitions ship with the package — no `@types` install:

```ts
import type { LatestRates, PairRate, DatedRates, RateEntry, HistoryQuery, RequestOptions } from 'central-bank-of-chile-exchange-rate';
```

## 📦 CommonJS

```javascript
const { getRate } = require('central-bank-of-chile-exchange-rate');

getRate('USD', 'CLP', { apiKey: 'art_live_...' }).then((pair) => console.log(pair.rate));
```

## 💡 Quota tips

- Rates change once per business day — cache the official table locally and a small monthly quota goes a long way.
- Every request counts toward your AllRatesToday quota, shared across all AllRatesToday endpoints on your key.

## 📖 Methods reference

| Method | Plan | Description |
| ------ | ---- | ----------- |
| `getRate(source, target, { apiKey })` | Free | Latest rate for one pair, resolved from the official table |
| `getLatestRates({ apiKey })` | Free | The central bank's full latest official table |
| `getRatesForDate(date, { apiKey, source?, target? })` | Paid | The official table (or one pair) for a YYYY-MM-DD date |
| `getHistory({ symbol \| source+target, from?, to? }, { apiKey })` | Paid | Daily series since 1982 |

## 📥 Bulk data (no key)

Need the whole archive rather than an API call? The same official tables are mirrored daily as open data:

- Hugging Face: [AllRatesToday/central-bank-exchange-rates](https://huggingface.co/datasets/AllRatesToday/central-bank-exchange-rates) — one CSV per institution (`rates/bcch.csv`)
- Kaggle: [allratestoday/central-bank-exchange-rates](https://www.kaggle.com/datasets/allratestoday/central-bank-exchange-rates)
- Raw JSON on GitHub: `https://raw.githubusercontent.com/AllRates-Today/central-bank-exchange-rates/main/data/bcch/latest.json`

## 🔗 Links

- **Website:** [allratestoday.com](https://allratestoday.com)
- [Central Bank of Chile rates page](https://allratestoday.com/central-bank-rates-api/bcch/) — live table, publication cadence, FAQ
- [All central bank sources](https://allratestoday.com/central-bank-rates-api/) · [Full list of 130+ central banks and tax authorities](https://allratestoday.com/central-bank-rates-api/institutions/) — one API, the same response shape for every source
- [Download central bank rates](https://allratestoday.com/download-central-bank-rates/) — every bank's latest table and history as Excel, CSV or JSON
- [Package docs on the site](https://allratestoday.com/docs/sdk/central-bank-of-chile-exchange-rate/) · [ERP integration guides](https://allratestoday.com/docs/integrations/)
- [API documentation](https://allratestoday.com/docs/#central-bank) · [Interactive reference](https://allratestoday.com/api-reference/) · [Methodology](https://allratestoday.com/official-rates-methodology/)
- [Register (Free)](https://allratestoday.com/register) · [Dashboard](https://allratestoday.com/profile) · [Pricing](https://allratestoday.com/pricing/)
- [Status](https://allratestoday.com/status)
- [Postman collection](https://allratestoday.com/postman/)
- [ChatGPT app](https://chatgpt.com/plugins/plugin_asdk_app_6ae1e76098f48191a285ac3f5ab7a83b) — ask ChatGPT for live and official central bank rates
- [OpenAPI reference on Bump.sh](https://bump.sh/allratestoday/doc/allratestoday-api) — also on [SwaggerHub](https://app.swaggerhub.com/apis-docs/allratestoday/allratestoday-exchange-rate-central-bank-rates-api/2.2.0)
- [GitHub](https://github.com/AllRates-Today/central-bank-of-chile-exchange-rate)

## 📜 License

MIT
