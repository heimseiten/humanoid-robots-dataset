# Humanoid Robots Dataset

An open, sourced index of 60 humanoid robots (manufacturer, country, locomotion, availability and price per market EU/US/CN, height, weight, named customers, confidence), maintained by [The Humanoid Report](https://www.thehumanoid.report/).

- Files: `humanoids.json`, `humanoids.csv` (identical content, one row per robot)
- Live source: https://www.thehumanoid.report/data/humanoids.json and `.csv`
- Snapshot date: see `generated` in the JSON (this repo is mirrored from the live site)
- Each robot has a `url` pointing to its page on the website with the underlying sources.

## Fields

| Field | Meaning |
|---|---|
| id, name, variant | Stable identifier, model name, variant |
| manufacturer, hq_country | Maker and headquarters country |
| group | Editorial group (`core` = main commercial candidates) |
| locomotion | e.g. biped, wheeled |
| status_EU / _US / _CN | Availability state per market (e.g. not_available, preorder, deployed_b2b) |
| price_*, currency_*, as_of_* | Price (empty if unknown), currency, month of the information |
| height (+unit), weight (+unit) | Manufacturer-stated dimensions |
| deployments, named_customers | Count and names of publicly named deployments |
| confidence | high / medium / low |
| last_reviewed | Date of last editorial check |
| url | Detail page with sources |

## Source principle
Facts only, each traceable to public sources listed on the robot's page. No images, no third-party text.

## License
[CC BY 4.0](LICENSE). Attribution required: credit "The Humanoid Report" and link to https://www.thehumanoid.report/ .

## Cite
The Humanoid Report. *Humanoid Robots Dataset* (2026). https://www.thehumanoid.report/ , https://github.com/heimseiten/humanoid-robots-dataset (CC BY 4.0). See `CITATION.cff`.
