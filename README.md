---
license: cc-by-4.0
language:
  - en
pretty_name: "Journeyed hotel facts and rankings: Los Angeles"
size_categories:
  - 10K<n<100K
task_categories:
  - question-answering
  - table-question-answering
tags:
  - hotels
  - travel
  - geospatial
  - los-angeles
configs:
  - config_name: los-angeles_hotels
    data_files: los-angeles/hotels.csv
  - config_name: los-angeles_facts
    data_files: los-angeles/facts.csv
  - config_name: los-angeles_questions
    data_files: los-angeles/questions.csv
  - config_name: los-angeles_rankings
    data_files: los-angeles/rankings.csv
  - config_name: los-angeles_anchors
    data_files: los-angeles/anchors.csv
---

# Journeyed hotel facts and rankings: Los Angeles

Hotels in Los Angeles with sourced facts (check-in and check-out times, parking, pets, breakfast, pool, Wi-Fi, accessibility and more), each with its source URL and the date it was checked, plus the 0 to 100 score per hotel and the full ranking for every published question. Built by Journeyed from open place data and facts read from hotels' own websites within robots.txt. No photos, reviews or copied text.

| File | What | Rows |
|---|---|---|
| [los-angeles/hotels.csv](los-angeles/hotels.csv) | Hotels in Los Angeles | 2660 |
| [los-angeles/facts.csv](los-angeles/facts.csv) | Sourced hotel facts, Los Angeles | 9556 |
| [los-angeles/questions.csv](los-angeles/questions.csv) | Questions and direct answers, Los Angeles | 345 |
| [los-angeles/rankings.csv](los-angeles/rankings.csv) | Full rankings per question, Los Angeles | 14100 |
| [los-angeles/anchors.csv](los-angeles/anchors.csv) | Anchors (airports, venues, areas), Los Angeles | 118 |
| [los-angeles/hotels.json](los-angeles/hotels.json) | Hotels, facts and rankings in one JSON file, Los Angeles |  |

Live copy, rebuilt with the site: https://journeyed.ai/data/open/README.txt

```text
Journeyed hotel facts and rankings: Los Angeles
===============================================

Hotels in Los Angeles with sourced facts (check-in and check-out times, parking, pets, breakfast, pool, Wi-Fi, accessibility and more), each with its source URL and the date it was checked, plus the 0 to 100 score per hotel and the full ranking for every published question. Built by Journeyed from open place data and facts read from hotels' own websites within robots.txt. No photos, reviews or copied text.

Version: 2026-10-03
Landing page: https://journeyed.ai/data/
Methodology: https://journeyed.ai/methodology/
License: Creative Commons Attribution 4.0 International (https://creativecommons.org/licenses/by/4.0/)
Attribute as: Journeyed (https://journeyed.ai/), CC BY 4.0, with a link to the hotel or question page where you use a row.

Contents
--------
- Los Angeles: 2660 hotels, 9556 sourced facts, 345 questions, 14100 ranking rows, 118 anchors

Los Angeles:
  https://journeyed.ai/data/open/los-angeles/hotels.csv     one row per hotel (place record, score, page URL)
  https://journeyed.ai/data/open/los-angeles/facts.csv      one row per sourced fact (value, source, license basis, checked date)
  https://journeyed.ai/data/open/los-angeles/questions.csv  one row per published question with its direct answer
  https://journeyed.ai/data/open/los-angeles/rankings.csv   the full ranking behind every question page
  https://journeyed.ai/data/open/los-angeles/anchors.csv    airports, venues and areas the questions are about
  https://journeyed.ai/data/open/los-angeles/hotels.json    all of the above in one JSON file

Metadata: https://journeyed.ai/data/open/datapackage.json (Frictionless Data Package, column types and descriptions), https://journeyed.ai/data/open/dataset.jsonld (schema.org Dataset), https://journeyed.ai/data/open/DATASHEET.txt.

Third-party data inside
-----------------------
Place records (name, address, coordinates, phone, website, category) come from Overture Maps Places release 2026-09-23.1, licensed CDLA-Permissive-2.0 (https://cdla.dev/permissive-2-0/). The record_source and record_license columns name it on every hotel row. Facts read from a hotel's website are facts (times, fees, yes/no amenities), never the site's wording, and each row links the page it came from.

Not included
------------
Photos, review text, guest opinion counts, verbatim policy sentences, licensed feeds, anything a hotel sent us through a claim, and coordinates that come from OpenStreetMap (ODbL is share-alike; those anchors link their OpenStreetMap source instead).

Corrections
-----------
A hotel or anyone else can correct a fact at https://journeyed.ai/claim/ or https://journeyed.ai/corrections/. The dataset is rebuilt with the site.
```
