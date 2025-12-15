
# LawDictionary dataset

**Overview**
- **Purpose**: A compiled legal-glossary dataset of short legal-term definitions intended to support searching, reference, and lightweight NLP tasks (e.g., glossary lookup, term normalization, simple training / fine-tuning for legal-domain models).
- **Language**: The definition texts in this folder are in Indonesian.

**Data Description**
- **Format**: JSON arrays. Each file contains an array of objects; the combined file is [LawDictionary/all.json](LawDictionary/all.json).
- **Record fields**: Most records contain a textual definition under the key **response**. Some entries may also include term labels or additional metadata depending on the source extraction.

**Directory Structure**
- **Files**: Individual letter-based files (e.g., `A.json`, `B.json`, ...) and a merged `all.json` containing all entries.
- **Location**: See [LawDictionary/all.json](LawDictionary/all.json) for the full dataset.

**Source & Attribution**
- **Original source**: Content was gathered from the public-facing dictionary at https://dictionary.law.com/Default.aspx.
- **Attribution**: If you redistribute or publish derived work, cite the original website as the source and confirm any copyright/licensing requirements before large-scale reuse.

**Intended Uses**
- **Reference**: Human-readable glossary for legal practitioners, students, and researchers.
- **NLP / Research**: Lightweight resource for term lookup, keyword expansion, training small domain-specific models, or building search indexes.
- **Data integration**: Can be merged into larger legal-corpus pipelines for annotation or cross-referencing.

**Usage Examples**
- **Inspect entries (Python)**:

```python
import json
from pathlib import Path

p = Path('LawDictionary/all.json')
data = json.loads(p.read_text(encoding='utf-8'))
print('Total entries:', len(data))
print('First entry keys:', list(data[0].keys()))
print('First definition:', data[0].get('response'))
```

- **Load and search (simple)**:

```python
term = 'abandon'
matches = [e for e in data if term.lower() in (e.get('response') or '').lower()]
```

**License & Notes**
- **Copyright**: The dataset was collected from the source linked above. Confirm copyright and terms-of-use before commercial redistribution or large-scale public sharing.
- **Quality**: Definitions are short explanatory texts; they may be paraphrased or localized. Treat this as a glossary, not legal advice.
- **Extending the dataset**: To add or correct entries, edit the appropriate letter file (e.g., `A.json`) and re-generate `all.json` if you maintain a single merged file.

If you'd like, I can also:
- generate a small script to search the dataset by term,
- add examples showing how to convert this dataset into a CSV or a SQLite lookup table,
- or commit the README changes to git for you.

