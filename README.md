# forin - A Foreign Investment Tracker using Apple Numbers

## Overview

This Apple Numbers spreadsheet helps track investments in foreign currency by calculating investment performance, FX rate differences, and nominal/percentage gains or losses.

## Why forin?

Why the name? **forin** is to **Foreign Investments** as **forex** is to **Foreign Exchange**!

Why this spreadsheet? Well, I recently started mutual fund investing in India using income earned in Ireland. As a foreign investor, two major variables affect my returns:

1. The volatility of the fund itself.
2. The volatility of currency exchange rates.

I’m more concerned about the latter, especially since there’s no easy way to visualize the gains or losses incurred due to currency fluctuations. That’s why I built this tool—to provide a structured view of the impact of exchange rate fluctuations on my investments. While it may not be flawless, it still offers a valuable overview.

## Features

- **Investment Tracking**: Log investment amounts in two user-defined currencies.
- **Foreign Exchange Rate Analysis**: See how bank charges and fund fees affect your investments.
- **Performance Monitoring**:
  - Displays current investment value in both currencies.
  - Calculates nominal and percentage gains/ losses in both currencies.
  - Predicts current effective FX rates based on historical differences.

## How to Use

1. **Download and open the Apple Numbers file.**
2. **Set Up the Spreadsheet**:
   - Fill in the settings table with your chosen currencies and ticker.
   - If needed, manually override the currency symbols (default: € & ₹).
3. **Input Investment Data**:
   - Use the Investments table. Some cells may auto-populate—override them if necessary.
4. **Track Performance and Analyze Trends**:
   - Monitor how both market performance and FX fluctuations impact your returns.

## Notes

- **Units are manually entered**, as they are calculated post-stamp-duty charges on the investment amount.

- Currency Definitions:

  - Currency 1 = Investment currency
  - Currency 2 = Foreign currency

- **Effective FX Rate**: Includes bank FX rates, bank fees, and fund stamp duty charges.

- `Predicted Current Effective FX Rate = (Current Actual FX Rate) - (Average FX Rate Difference)`

- `Current Foreign Currency Value = (Investment Currency Value) / (Predicted Current Effective FX Rate)`

- **FX Rate Differences [LIMITATION]**:

  - These differences are sensitive to the actual amount converted; this works well when the investment & potential withdrawal amounts remains relatively static.
  - If investment & withdrawal amounts would fluctuate significantly, a **weighted approach** should be applied to ensure proportional allocation of bank and fund charges. This spreadsheet does not do that yet!

## License

MIT No Attribution

Copyright 2025 Kavith Kamaraj

Permission is hereby granted, free of charge, to any person obtaining a copy of this
software and associated documentation files (the "Software"), to deal in the Software
without restriction, including without limitation the rights to use, copy, modify,
merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
