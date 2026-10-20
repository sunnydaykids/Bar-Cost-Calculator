# Bar Cost Calculator

A small, mobile-friendly web app for calculating ingredient cost and menu prices for draft beer and liquor.

## Features
- Draft beer: enter a beer name and prices for sixth-, quarter-, and half-barrel kegs.
- Calculates cost per ounce, configurable pint and tall pour costs, and menu prices at 20%, 25%, and 30% ingredient cost.
- Liquor: enter prices for 750 mL and/or 1 liter bottles.
- Calculates cost per ounce, theoretical 1.5 oz shot count (customizable), cost per shot, and menu prices at 20%, 25%, and 30% ingredient cost.
- Displays exact suggested price and a convenience price rounded up to the next $0.25.
- Can be hosted on GitHub Pages and added to an iPhone Home Screen.

## Keg capacities
Uses the working values requested: 665 fl oz (sixth barrel), 992 fl oz (quarter barrel), and 1,984 fl oz (half barrel). Actual sellable yield can be lower due to foam, line loss, and waste.

## Bottle conversions
Uses 1 US fl oz = 29.5735295625 mL. A 750 mL bottle is about 25.36 fl oz and a 1 liter bottle is about 33.81 fl oz.

## Menu-price math
Target price = ingredient cost per drink ÷ target ingredient-cost percentage.
For example, a $1 ingredient cost at 25% cost implies a $4 menu price before taxes, overhead, comps, waste, and other considerations.

## Publish on GitHub Pages
1. Create a new repository, e.g. `bar-cost-calculator`.
2. Upload `index.html`, `manifest.json`, `sw.js`, and `README.md` directly into the repository root (do not upload the ZIP itself).
3. In Settings → Pages, set Source to “Deploy from a branch”, choose branch `main` and folder `/(root)`, then Save.
4. Wait for the published URL, usually `https://YOUR-USERNAME.github.io/bar-cost-calculator/`.
5. On iPhone, open that URL in Safari → Share → Add to Home Screen.

## Notes
- Calculations happen in the browser. The app does not store drink prices, connect to accounts, or transmit data.
- The app is a calculator, not a complete beverage-cost model. It does not account for sales tax, garnish/mixers, spillage, line loss, comps, or discounts.
