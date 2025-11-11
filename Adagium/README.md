# Indo Legal Corpus - Adagium (Legal Maxims) Documentation

## Overview
This dataset (`all.json`) contains a comprehensive collection of Latin legal maxims (adagium) commonly used in Indonesian legal practice and jurisprudence. It serves as a reference guide for legal terminology and foundational principles in law.

## File Structure
- **Format**: JSON array
- **Total Entries**: 100+ legal maxims
- **Language**: Indonesian (with Latin original terms)

## Data Schema

Each entry contains three fields:

| Field | Type | Description |
|-------|------|-------------|
| `instruction` | String | The Latin legal maxim in its original form with Indonesian translation request |
| `context` | String | Classification category: "Istilah Hukum / Adagium" (Legal Terms / Maxims) |
| `response` | String | Indonesian explanation and meaning of the legal maxim |

## Purpose & Use Cases

### Legal Education & Training
- Serves as a reference material for law students and practitioners
- Helps understand foundational legal principles and their Latin terminology
- Facilitates learning of traditional legal concepts applied in Indonesian courts

### Jurisprudence & Practice
- Provides standardized interpretation of commonly cited legal principles
- Supports legal argumentation and case analysis
- Enables consistency in legal reasoning across Indonesian judicial system

### AI/ML Applications
- Training dataset for legal question-answering systems
- Development of Indonesian legal knowledge bases
- Building legal chatbots and automated legal research tools
- NLP model training for legal terminology recognition

## Coverage Areas

The dataset covers major legal domains including:
- **Procedural Law**: Evidence handling, burden of proof, judicial impartiality
- **General Principles**: Justice, equality before law, legal remedies
- **Contract Law**: Pacta sunt servanda (binding nature of agreements)
- **Criminal Law**: Presumption of innocence, punishment proportionality
- **Administrative Law**: Government legitimacy, legal hierarchy
- **International Law**: Territory jurisdiction, treaty obligations

## Source Information

**Primary Source**: HukumOnline Blog  
**URL**: https://www.hukumonline.com/berita/a/adagium-hukum-lt619387d0b9e9c/  
**Collection Method**: Web scraping from legal education and reference materials

## Key Maxims Included

Notable examples:
- **"Nemo judex in causa sua"** - Judge cannot rule on own case
- **"Pacta sunt servanda"** - Agreements must be honored
- **"Fiat justitia ruat coelum"** - Justice must prevail regardless of consequences
- **"Ignorantia juris non excusat"** - Ignorance of law is not an excuse
- **"Audi et alteram partem"** - Hear both sides of dispute
- **"Presumption of innocence"** - Accused is innocent until proven guilty

## Data Quality Notes

- Entries are formatted consistently with Latin terms and Indonesian translations
- Explanations provide practical legal context relevant to Indonesian legal system
- Some maxims may have variations in Latin spelling (historical usage)
- All translations follow established Indonesian legal doctrine

## Usage Recommendations

1. **Academic Reference**: Suitable for legal education and research
2. **System Integration**: Can be incorporated into legal information systems
3. **Training Data**: Appropriate for supervised ML tasks in legal NLP
4. **Knowledge Base**: Serves as foundation for legal expert systems

## Maintenance & Updates

- Dataset reflects Indonesian legal interpretation standards
- May require periodic updates as legal practices evolve
- Entries are based on established jurisprudential sources
- Suitable for version control and documentation alongside legal corpus projects