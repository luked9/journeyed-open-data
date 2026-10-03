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
| [los-angeles/hotels.csv](los-angeles/hotels.csv) | Hotels in Los Angeles | 2612 |
| [los-angeles/facts.csv](los-angeles/facts.csv) | Sourced hotel facts, Los Angeles | 10421 |
| [los-angeles/questions.csv](los-angeles/questions.csv) | Questions and direct answers, Los Angeles | 749 |
| [los-angeles/rankings.csv](los-angeles/rankings.csv) | Full rankings per question, Los Angeles | 23886 |
| [los-angeles/anchors.csv](los-angeles/anchors.csv) | Anchors (airports, venues, areas), Los Angeles | 118 |
| [los-angeles/hotels.json](los-angeles/hotels.json) | Hotels, facts and rankings in one JSON file, Los Angeles |  |

Live copy, rebuilt with the site: https://journeyed.org/data/open/README.txt

```text
Journeyed hotel facts and rankings: Los Angeles
===============================================

Hotels in Los Angeles with sourced facts (check-in and check-out times, parking, pets, breakfast, pool, Wi-Fi, accessibility and more), each with its source URL and the date it was checked, plus the 0 to 100 score per hotel and the full ranking for every published question. Built by Journeyed from open place data and facts read from hotels' own websites within robots.txt. No photos, reviews or copied text.

Journeyed is an independent guide to hotels in Los Angeles, built from sourced facts and reader votes. Get to know the details.

Version: 2026-10-03
Landing page: https://journeyed.org/data/
Methodology: https://journeyed.org/methodology/
License: Creative Commons Attribution 4.0 International (https://creativecommons.org/licenses/by/4.0/)
Attribute as: Journeyed (https://journeyed.org/), CC BY 4.0, with a link to the hotel or question page where you use a row.

Contents
--------
- Los Angeles: 2612 hotels, 10421 sourced facts, 749 questions, 23886 ranking rows, 118 anchors

Los Angeles:
  https://journeyed.org/data/open/los-angeles/hotels.csv     one row per hotel (place record, score, page URL)
  https://journeyed.org/data/open/los-angeles/facts.csv      one row per sourced fact (value, source, license basis, checked date)
  https://journeyed.org/data/open/los-angeles/questions.csv  one row per published question with its direct answer
  https://journeyed.org/data/open/los-angeles/rankings.csv   the full ranking behind every question page
  https://journeyed.org/data/open/los-angeles/anchors.csv    airports, venues and areas the questions are about
  https://journeyed.org/data/open/los-angeles/hotels.json    all of the above in one JSON file

Metadata: https://journeyed.org/data/open/datapackage.json (Frictionless Data Package, column types and descriptions), https://journeyed.org/data/open/dataset.jsonld (schema.org Dataset), https://journeyed.org/data/open/DATASHEET.txt.

Third-party data inside
-----------------------
Place records (name, address, coordinates, phone, website, category) come from Overture Maps Places release 2026-09-23.1, licensed CDLA-Permissive-2.0 (https://cdla.dev/permissive-2-0/). The record_source and record_license columns name it on every hotel row. Facts read from a hotel's website are facts (times, fees, yes/no amenities), never the site's wording, and each row links the page it came from.

Not included
------------
Photos, review text, guest opinion counts, verbatim policy sentences, licensed feeds, anything a hotel sent us through a claim, and coordinates that come from OpenStreetMap (ODbL is share-alike; those anchors link their OpenStreetMap source instead).

Corrections
-----------
A hotel or anyone else can correct a fact at https://journeyed.org/claim/ or https://journeyed.org/corrections/. The dataset is rebuilt with the site.
```
