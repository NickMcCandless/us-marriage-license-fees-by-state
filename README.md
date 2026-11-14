# Marriage license fees, waiting periods and validity by U.S. state

The marriage license fee, waiting period and how long a license is valid in the 50 states and the District of Columbia, restated from official state and county pages, with the page and the date it was read. Each row links the official page each figure was read on and the Wedding Remedy state page that covers the rest of that state's rules.

Published by Wedding Remedy, which is operated by Eltherion, LLC. Wedding Remedy is not a law firm and does not provide legal, tax, or financial advice.

## Canonical page

https://weddingremedy.com/guides/marriage-license

The page shows: Published October 30, 2026. Updated November 12, 2026. Last verified November 12, 2026.

## File

The file was downloaded on 2026-11-13 and is kept exactly as published. The file name is the download name the site sends. Its SHA-256 checksum is in `CHECKSUMS.txt`.

| File | Published at | Data rows | Columns |
| --- | --- | --- | --- |
| `data/marriage-license-fees-by-state.csv` | https://weddingremedy.com/guides/marriage-license/fees.csv | 51 | 20 |

The file has one header line and uses CRLF line endings. Several text cells contain commas and are quoted.

## Source of the underlying records

Each state's official marriage license pages: official state and county pages, linked in the file. The guide says the table is built "from official state and county pages" and that the CSV has "the source and the date read beside the fee, the waiting period and the validity period."

The date each source was checked is in the file itself, in the `fee_checked`, `waiting_period_checked` and `validity_checked` columns. In this copy every one of those dates is 2026-10-30 or 2026-11-12.

## Columns

| Column | Meaning | First row (Alabama) or example | Blank cells |
| --- | --- | --- | --- |
| `state` | State name, or District of Columbia | `Alabama` | 0 |
| `code` | Two-letter postal code | `AL` | 0 |
| `fee` | The fee as the guide's table shows it | `$73`; Delaware is `$70 resident, $120 non-resident` | 0 |
| `fee_usd` | The fee as a number, where it is one plain amount | `73` | 3 |
| `fee_detail` | The fee as the official page states it, in a sentence | `Alabama issues no marriage license. Mobile County Probate Court charges $73 to record the Alabama Marriage Certificate form; each county probate court sets its own recording fee.` | 0 |
| `fee_set_by` | `state` or `county` | `county` | 4 |
| `fee_county` | The county whose fee is shown, where the row shows one county's fee | `Mobile` | 22 |
| `fee_source` | URL of the official page the fee was read on | `https://probate.mobilecountyal.gov/public-records/document-recording` | 0 |
| `fee_checked` | Date that page was read, as YYYY-MM-DD | `2026-11-12` | 0 |
| `waiting_period` | The waiting period as the guide's table shows it | `3 days` (Alaska); `None` (Arizona) | 1 |
| `waiting_days` | The waiting period as a number of days; `0` where the table shows None | `3` (Alaska) | 1 |
| `waiting_period_detail` | The waiting period rule in a sentence | `Three business days after a completed application is received by the issuing office.` (Alaska) | 1 |
| `waiting_period_source` | URL of the official page the waiting period was read on | `https://health.alaska.gov/en/services/marriage-license/` (Alaska) | 1 |
| `waiting_period_checked` | Date that page was read, as YYYY-MM-DD | `2026-10-30` (Alaska) | 1 |
| `valid_for` | How long the license is valid, as the guide's table shows it | `90 days` (Alaska); `Does not expire` (Georgia) | 1 |
| `valid_days` | The validity period as a number of days, where `valid_for` is a number of days | `90` (Alaska) | 15 |
| `validity_detail` | The validity rule in a sentence | `No license is issued. The notarized Alabama Marriage Certificate form must be delivered to a probate court within 30 days of the later spouse signature.` | 0 |
| `validity_source` | URL of the official page the validity rule was read on | `https://www.alabamapublichealth.gov/vitalrecords/marriage-faqs.html` | 0 |
| `validity_checked` | Date that page was read, as YYYY-MM-DD | `2026-10-30` | 0 |
| `state_page` | The state's page on weddingremedy.com | `https://weddingremedy.com/guides/marriage-license/alabama` | 0 |

Blank cells follow what the guide's table shows. `fee_usd` is blank for Delaware, Indiana and South Carolina, where the fee differs by residency. The Alabama row has no waiting period or validity period figure; the guide's table shows "See the state page" for both. `valid_days` is blank where `valid_for` is `1 year`, `6 months` or `Does not expire`, and for Alabama.

## Method and caveats stated on the live page

From the guide:

> Where counties set the fee, the table shows one county's fee: the largest county's where its official page could be read, otherwise another county's. The state page names the county. "See the state page" means the rule is not one plain figure, or no official page we could read stated it: the state page shows the wording or the official page to ask. Rules change, so confirm with the clerk where you apply.

> A row links the official page its fee was read on, with the day the row was last verified; the state page links the sources of the other rules.

- "Where counties set the fee, the figure is one county's, named on the state page."
- Some states have no waiting period "in some cases only for adults or with conditions the state page explains."
- The state pages say: "Rules and fees change, and this is not legal advice: confirm with the clerk where you apply before you rely on a rule."
- "Wedding Remedy is not a law firm and does not provide legal, tax, or financial advice."

Wedding Remedy's editorial standards say the state-by-state marriage license pages "state a fee, a waiting period or a document list only as one official page states it, link that page with the day it was read, and say to check with the county clerk where no official page could be read."

## Updates

The guide states no fixed update schedule. Each row carries the date its sources were read, and the guide shows its Published, Updated and Last verified dates. The editorial standards say a guide's Updated date "changes only for a substantive revision." The file in this repository is the copy downloaded on 2026-11-13; the page above has the latest data.

## How to cite

The guide says the table is "Free to cite with a link to this page." For example:

> Wedding Remedy. Marriage license fees, waiting periods and validity by U.S. state. Last verified November 12, 2026. https://weddingremedy.com/guides/marriage-license

A machine-readable citation is in `CITATION.cff`.

## License

This compilation is released under the Creative Commons Attribution 4.0 International license (CC BY 4.0); see `LICENSE`. Credit Wedding Remedy with a link to https://weddingremedy.com/guides/marriage-license. The underlying fees and rules are public information published by the state and county offices linked in each row.

## Corrections

From the editorial standards: "If something in a guide is wrong, email help@weddingremedy.com."
