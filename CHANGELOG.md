# Changelog

## 1.6.0
- **Corporate Action Support:** Added support for the "Merged(Acquisition)" action type to ensure accurate portfolio tracking and calculations during corporate restructurings like exchange listing migrations.
- **Summary Section:** Introduced a "Summary" section in the header for a high-level overview of total share quantities and deposits (Electronic Fund Transfer) made during the period covered by uploaded statements.
- **Unsupported Action Alerts:** Added an alert to flag corporate actions that are not yet implemented, identifying the exact lines from the statement to help you report them.
- **Expanded EEA Support:** Extended coverage from EU to EEA (European Economic Area) to include the EEA EFTA states (Norway, Iceland, and Liechtenstein).
- **Comprehensive Market Coverage:** Added 43 new exchanges (24 EEA and 19 Non-EEA) based on IBKR's official directory.
- **Default Year Selection:** Automatically preselects the previous taxable year for sold stocks and received dividends when that data is present in imported reports, minimizing the risk of auto-filling incorrect information.
- **Year-Specific Visuals:** Updated the color scheme to help users easily distinguish the 2025 version from the 2024 taxation year extension.
- **Improved Data Parsing:** Fixed a bug in IBKR activity reports to correctly process number formatting for thousands, ensuring data is imported accurately.

## 1.5.1
- Bug fix: Fractional shares are now rounded correctly to 5 decimal places.
-	Bug fix: Year-based sales filtering wasn't applied when filling out the form - now fixed.

## 1.5.0
- Added support for retaining imported CSV statements data in the extension's session storage. This improves the user experience by eliminating the need to re-select files each time the popup is opened (due to browser extension limitations).
- Added a "Delete Data" button to manually clear stored data after use.

## 1.4.0
- Improve the clarity and readability of the tables.

## 1.3.2
- Introduce stock split basis adjustment/allocation. It refers to the process of redistributing the original cost of acquisition across the increased number of shares following a split. The key principle is that the total acquisition cost remains unchanged—only the cost per share is adjusted based on the new share count. Since a split does not introduce newly purchased shares, but rather restructures existing ones, it is not considered a separate acquisition event.

## 1.3.1
- Bug fix: The sales basis cost should be calculated as the sum of all acquisition prices in BGN (with the acquisition date determining the currency fixation), applying FIFO. This ensures that the realized profit/loss reflects the impact of currency fluctuations.

## 1.3.0
- Minor UI adjustments.

## 1.2.0
- Only the auto-fill options relevant to the selected view are enabled.
- Disabled view when no records are present.

## 1.1.0
- Moved the Auto-Fill options to a dropdown menu.
- Split the Sales auto-fill into two options: "Fill Sales Outside the EEA (Annex 5)" and "Fill Sales From the EEA (Annex 13)".
- Highlighted EEA stock exchanges in blue in the "Sold Stocks" table and added a disclaimer for clarification.

## 1.0.3
- Calculate cumulative buy/sell prices and realized P/L, since the NRA portal doesn't allow submitting multiple lines with code 508 in Annex 5, Part I, Table II. 🤷🏻‍♂️
- Add a Non-EEA/EEA filter to the sold stocks view, since Annex 5, Part I, Table II applies to sales on Non-EEA stock exchanges. Sales of stocks purchased on EEA stock exchanges should be reported in Annex 13, Part II, under code 508 (TODO).

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