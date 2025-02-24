# Construction Item Description Standardization

## Overview
This notebook implements a comprehensive standardization system for construction item descriptions. It addresses common challenges in construction inventory management by cleaning, standardizing, and deduplicating item descriptions.

## Key Features
1. **Description Standardization**
  - Standardizes measurements (inches, feet, metric)
  - Normalizes unit representations
  - Handles construction-specific terminology
  - Standardizes brand names and common abbreviations

2. **Deduplication Processing**
  - Identifies and removes duplicate items
  - Groups similar items
  - Maintains original SKUs and descriptions
  - Creates reference tables for duplicate tracking

3. **Output Tables**
  - `inscope_items_unique`: Clean, deduplicated items
  - `inscope_items_duplicates`: Identified duplicates for review
  - Includes detailed analysis of standardization results

## Usage
This notebook processes construction item descriptions from the Lakehouse table 'inscope_items_output' and generates standardized outputs with duplicates removed. It helps maintain data consistency and reduce inventory redundancy.

## Requirements
- Input table must contain an 'item_description' column
- Dependencies: pandas, numpy, re (regex)
- Microsoft Fabric Lakehouse environment

## Note
The standardization rules are customizable and can be extended based on specific needs and patterns in your construction item inventory.