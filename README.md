# SRD Reference Data

D&D 5th Edition System Reference Document content, compiled for use by Dalang apps. Covers both the 2014 and 2024 rules, organized by version so each stays separate.

## What's here

Plain JSON files, one category per file, grouped under a folder per SRD version (`2014/`, `2024/`). Each version folder has its own `manifest.json` noting the source and last-updated date.

Currently included: Conditions. More categories will be added over time.

## Source

The game rules text in this data comes from the official D&D 5th Edition System Reference Document, published by Wizards of the Coast:

- SRD 5.1 (2014 rules): https://www.dndbeyond.com/srd
- SRD 5.2.1 (2024 rules): https://www.dndbeyond.com/srd

Both are licensed under the Creative Commons Attribution 4.0 International License (CC-BY-4.0). See `LICENSE.md` for the full attribution notice.

Data was checked against two open-source community projects that structure the same SRD text as JSON, credited here for that structuring work (their own code and data organization, not the underlying game rules, which remain Wizards of the Coast's):

- [5e-bits/5e-database](https://github.com/5e-bits/5e-database) (MIT License)
- [open5e/open5e-api](https://github.com/open5e/open5e-api) (MIT License)

## License

Game rules text: © Wizards of the Coast, used under CC-BY-4.0. See `LICENSE.md`.

Everything else in this repository (the compiled JSON structure, this README): MIT License.

## Using this data

Each entry follows a simple shape:

```json
{
  "index": "blinded",
  "name": "Blinded",
  "desc": ["- line one", "- line two"],
  "url": "dalang/2024/conditions/blinded"
}
```

`desc` is always an array of strings, one bullet point per line, matching how the rules text is actually written.
