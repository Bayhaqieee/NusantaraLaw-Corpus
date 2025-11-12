# Indo Legal Corpus - Istilah Hukum (Legal Terms) Documentation

## Overview

This dataset contains a comprehensive collection of Indonesian legal terminology (*Istilah Hukum*) with their official definitions. It serves as a vital reference guide for understanding the vocabulary used in Indonesian court proceedings, legislation, and general legal practice. The definitions cover various aspects of law including criminal, civil, procedural, and administrative law.

## File Structure

* **Format**: JSON array
* **Total Entries**: 100+ legal terms
* **Language**: Indonesian

## Data Schema

Each entry contains three fields:

| Field | Type | Description |
| --- | --- | --- |
| `instruction` | String | The specific legal term requesting definition (e.g., "Jelaskan definisi dari istilah hukum 'Abolisi'.") |
| `context` | String | Classification category: "Istilah Hukum" (Legal Terms) |
| `response` | String | The comprehensive legal definition and explanation of the term |

## Purpose & Use Cases

### Legal Education & Public Awareness

* **Student Reference**: Essential glossary for law students to master technical vocabulary.
* **Public Literacy**: Helps the general public understand complex legal language used in court documents or news.
* **Court Transparency**: Supports the judicial mission to make legal proceedings more accessible to non-lawyers.

### Professional Legal Practice

* **Standardization**: Provides a standardized set of definitions accepted by the High Court (Pengadilan Tinggi).
* **Document Drafting**: Assists paralegals and junior lawyers in drafting precise legal documents.
* **Procedural Clarity**: Clarifies distinct procedural steps (e.g., *Minutasi*, *Eksekusi*) to ensure compliance.

### AI/ML Applications

* **Legal NLP**: Excellent training data for Indonesian Legal LLMs to understand entity extraction.
* **Automated Assistance**: Backbone for legal chatbots answering "What does X mean?" questions.
* **Semantic Search**: Enhances search engines by mapping legal queries to their correct formal definitions.

## Coverage Areas

The dataset covers major legal domains including:

* **Criminal Law (Pidana)**: Terms like *Delik* (offenses), *Amnestie*, *Abolisi*, and specific types of crimes.
* **Civil Law (Perdata)**: Concepts regarding contracts, *Wanprestasi* (default), and *Ganti Rugi* (damages).
* **Procedural Law (Hukum Acara)**: Court processes such as *Kasasi*, *Banding*, *Eksepsi*, and *Pembuktian* (evidence).
* **Bankruptcy (Kepailitan)**: Terms related to insolvency, *Kurator*, and creditors (*Konkuren*, *Separatis*).
* **Court Administration**: Internal court functions like *Minutasi perkara* and *Panitera*.

## Source Information

**Primary Source**: Pengadilan Tinggi Sulawesi Tenggara (High Court of Southeast Sulawesi)

**URL**: [https://www.pt-sultra.go.id/main/index.php/pengumuman/7-kamus-hukum](https://www.pt-sultra.go.id/main/index.php/pengumuman/7-kamus-hukum)

**Collection Method**: Web scraping from the official provincial government judiciary website

## Key Terms Included

Notable examples:

* **"Abolisi"** - Elimination of all consequences of a criminal judgment.
* **"Ne bis in idem"** - Principle that no one can be tried twice for the same offense.
* **"Actio in pauliana"** - Legal action to void acts by a debtor that harm the creditor.
* **"Force Majeure (Keadaan Kahar)"** - Unforeseeable circumstances preventing contract fulfillment.
* **"Beban pembuktian terbalik"** - Reverse burden of proof (accused must prove innocence).
* **"Vrijspraak"** - Acquittal/Exoneration from all charges.
* **"Class Action"** - Lawsuit filed by a group representing a larger class of people.

## Data Quality Notes

* **Official Definitions**: Definitions are sourced directly from a judicial body, ensuring high reliability.
* **Formal Language**: Uses formal Indonesian legal syntax appropriate for professional settings.
* **Cross-Referencing**: Some definitions reference specific codes (e.g., KUHPerdata, KUHAP) for further context.
* **Formatting**: JSON structure is clean and ready for immediate ingestion into databases or training pipelines.

## Usage Recommendations

1. **Information Retrieval**: Build a dictionary or glossary feature for legal apps.
2. **Context Augmentation**: Use in RAG (Retrieval-Augmented Generation) systems to provide context for AI generating legal advice.
3. **Training Data**: Fine-tune language models to distinguish between similar terms (e.g., *Delik aduan* vs *Delik biasa*).
4. **Educational Tools**: Create flashcards or quiz systems for law students.

## Maintenance & Updates

* **Jurisdictional Updates**: While definitions are generally universal in Indonesia, specific statutes referenced may evolve.
* **Source Monitoring**: Periodic checks of the PT Sultra website are recommended to capture new terms or revisions.
* **Version Control**: Best maintained as a static corpus unless significant legislative changes occur (e.g., updates to the KUHP).