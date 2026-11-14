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

## PFLS Intelligence 2.0
- Experimental zone-quality score based on candle displacement and range; it is a ranking aid, not a win probability.
- Cross-timeframe confluence counts overlapping fresh zones of the same type across different timeframes.
- Market-structure observations compare the latest two confirmed swing highs and lows on each loaded timeframe.
- Optional browser notifications can alert when price approaches an active fresh zone, using recent M5 candle range as an approximate distance threshold.
- Zone inventory is saved locally in the browser (up to 600 records) and restored on refresh. Browser storage is device/browser-specific and may be cleared by the user or operating system.

## Important research limitations
The zone detector remains experimental and is based on local candle pivots plus a displacement candle; it is not a validated institutional supply/demand definition. The first later candle overlap marks a zone as touched/mitigated, including a wick touch. Only untouched zones remain in the active inventory; touched zones remain in local research history. Confluence requires price-range overlap and does not imply that a zone will hold. Structure readings are simplified swing comparisons, not confirmed trend forecasts. Notification support depends on browser permission and platform behavior. Candle feed/API compatibility must be tested on the target browser. No win rate is claimed.

## Project independence
This repository is separate from `PFLS-Trader-EA` and does not modify or import its application files.
