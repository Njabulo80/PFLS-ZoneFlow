# Njabulo FX — PFLS ZoneFlow

Independent Android-friendly web app for multi-timeframe supply and demand zone research on Deriv Volatility 75 Index (`R_75`).

## Deploy with GitHub Pages
1. Open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **main** and folder **/(root)**, then Save.
4. After GitHub publishes the site, open the Pages URL on Android Chrome and use **Add to Home screen** / **Install app**.

## Initial version
- Public Deriv market-data connection; no account login required.
- Eight timeframe candle histories: W1, D1, H4, H1, M30, M15, M5, M1.
- Separate fresh supply and demand inventory, counts per timeframe, and proximity ranking.
- First later candle overlap marks a zone as touched/mitigated; separate timeframe zones remain independent.
- Research-only. No order placement, no account credentials, and no verified win-rate claim.

## Important research limitations
The initial zone detector is experimental and based on local candle pivots plus a displacement candle. It is not yet a validated institutional supply/demand definition. The first-touch rule is applied to later candles in the loaded history. Refreshing the page currently rebuilds the in-memory zone inventory; persistent research history and robust zone identity are planned for a later version. Candle feed/API compatibility must be tested on the target browser.

## Project independence
This repository is separate from `PFLS-Trader-EA` and does not modify or import its application files.
