# Changelog

## 1.3.0
- Minor UI adjustments.

## 1.2.0
- Only the auto-fill options relevant to the selected view are enabled.
- Disabled view when no records are present.

## 1.1.0
- Moved the Auto-Fill options to a dropdown menu.
- Split the Sales auto-fill into two options: "Fill Sales Outside the EU (Annex 5)" and "Fill Sales From the EU (Annex 13)".
- Highlighted EU stock exchanges in blue in the "Sold Stocks" table and added a disclaimer for clarification.

## 1.0.3
- Calculate cumulative buy/sell prices and realized P/L, since the NRA portal doesn't allow submitting multiple lines with code 508 in Annex 5, Part I, Table II. 🤷🏻‍♂️
- Add a Non-EU/EU filter to the sold stocks view, since Annex 5, Part I, Table II applies to sales on Non-EU stock exchanges. Sales of stocks purchased on EU stock exchanges should be reported in Annex 13, Part II, under code 508 (TODO).

## 1.0.2
- Add IBIS and IBIS2 (Deutsche Börse Xetra) as separate stock exchanges.

## 1.0.1
- Bug fix: Properly handle empty columns when parsing the CSV files.

## 1.0.0
- Bug fixes
- Added a how-to-use demo video

## 0.6.1 Beta
- Fix inconsistent language indicator

## 0.6.0 Beta
- Highlight the action button while prefilling the table
- Prefill Annex 8, Part I starting from the end of the list in case there are already filled rows

## 0.5.2 Beta
- Increase decimal precision for the exchange
- Bug fixes

## 0.5.1 Beta
- Bug fixes

## 0.5.0 Beta
- Year-based filter for the "Sold Stocks" table
- Added a language toggle to the header
- UI improvements

## 0.4.0 Beta
- Sales view
- Auto-prefill for NRA's Annex 5, Part I, Table II - taxable income from the sale or exchange of shares

## 0.3.1 Beta
- Persist the user's language preference using the [Chrome Storage API](https://developer.chrome.com/docs/extensions/reference/api/storage).

## 0.3.0 Beta
- Added a language toggle to switch between English and Bulgarian.
- Changed the font to Sofia Sans, which supports Cyrillic characters.

## 0.2.0 Beta
- UI improvements

## 0.1.0 Beta
- IBKR CSV statement processing
- Stock Acquisitions view
- Received Dividend view with year-based filtering
- Auto-prefill for NRA's Annex 8, Part I
- Auto-prefill for NRA's Annex 8, Part III