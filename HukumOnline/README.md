# HukumOnline Dictionary (NusantaraLaw Corpus)

This folder contains an Indonesian legal dictionary dataset sourced from HukumOnline.

## What it is
- A collection of JSON files (`A.json`, `B.json`, ..., `Z.json`, plus `all.json`) with legal terms and their definitions.
- Each entry includes a short description suitable for dictionary lookup, NLP datasets and legal knowledge retrieval.

## Why it exists
- To support legal tech and NLP projects for Indonesian law.
- To provide a structured, searchable vocabulary of Indonesian legal concepts (adopsi, definisi, dan istilah hukum).

## How to use
- `all.json` is the complete dictionary.
- `A.json`..`Z.json` are alphabetically partitioned subsets for convenience.
- Load these JSON files in your code (Python, JS, etc.) and index or search by `response`/term.

## Notes
- Entries may be complete or in-progress; the dataset is intended as a reference and training resource.
- Keep the JSON format unchanged when editing to avoid parse issues.

## License
- Check project root `LICENSE_DATA.txt` and repository-wide license terms for usage permissions.
