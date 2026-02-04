# Document AI to AI_EXTRACT Migration Demo

## Helpful Links

- [Deprecation Notice](https://docs.snowflake.com/en/release-notes/bcr-bundles/un-bundled/bcr-2156)
- [AI_EXTRACT Documentation](https://docs.snowflake.com/en/sql-reference/functions/ai_extract)
- [Arctic Extract Public Blog](https://www.snowflake.com/en/engineering-blog/arctic-extract-document-understanding/)
- [Fine-tuning arctic-extract models](https://docs.snowflake.com/en/user-guide/snowflake-cortex/arctic-extract-finetuning)

---

## Overview

This notebook demonstrates the migration path from the deprecated Document AI `model!PREDICT` method to the new `AI_EXTRACT` function. It serves as both a migration guide and a showcase of AI_EXTRACT's capabilities.

## What's Covered

### 1. Environment Setup
- Database and schema creation (AI_EXTRACT_WALKTHROUGH)
- Stage setup for document storage
- File upload patterns using Snowpark

### 2. Deprecated Document AI (model!PREDICT)
- Example of the old Document AI approach
- Using trained models with `model!PREDICT`
- Why this method is being deprecated (BCR-2156)

### 3. Migration to AI_EXTRACT
- Zero-shot extraction (no training required)
- Transition from Arctic-TILT to Arctic-extract vision model
- Side-by-side comparison of old vs new approaches

### 4. AI_EXTRACT Response Formats
- Array of arrays syntax
- Object syntax with field descriptions
- Simple array format
- JSON schema for complex extractions

### 5. Image Table Extraction Examples
Four progressively complex table extraction demos:
- **Simple Table**: Basic gene/CpG site data
- **Dual-Column Table**: Sequence identity comparisons across species
- **Multi-Layer Nested Table**: Tumor characteristics with demographic groupings
- **Free-Text Table**: Systematic review data with narrative content
