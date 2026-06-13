---
title: Quote Analysis Engine
filename: quote-analysis-engine.md
version: 1.0
skill_type: pseudo-tool
description: Extracts and normalises builder quote details for structured comparison in the Homebuilder Copilot.
---

## Purpose

Extract structured information from builder quotes and produce a normalised comparison across multiple builders.  
This enables the Homebuilder Copilot to highlight inclusions, exclusions, provisional sums, hidden costs, and scope gaps.

---

## Behaviour

When the user uploads or pastes a quote:

- Extract inclusions  
- Extract exclusions  
- Identify provisional sums  
- Identify hidden costs  
- Identify scope gaps  
- Normalise categories across builders  
- Flag ambiguous or missing items  
- Do not guess or fabricate numbers  

If multiple quotes are provided:

- Produce a side‑by‑side comparison  
- Align categories so the user can compare “apples to apples”  

---

## Output Format

Use the following structured format for all quote comparisons:

### Quote Comparison

| Category           | Builder A | Builder B | Notes |
|--------------------|-----------|-----------|-------|
| Inclusions         | ...       | ...       | ...   |
| Exclusions         | ...       | ...       | ...   |
| Provisional sums   | ...       | ...       | ...   |
| Hidden costs       | ...       | ...       | ...   |
| Scope gaps         | ...       | ...       | ...   |
| Total price        | ...       | ...       | ...   |

If only one quote is provided, output this simplified version:

### Quote Breakdown

- Inclusions:  
- Exclusions:  
- Provisional sums:  
- Hidden costs:  
- Scope gaps:  
- Total price:  

---

## Extraction Rules

### Inclusions

Items explicitly included in the contract price.

### Exclusions

Items the builder has not priced or has left out.

### Provisional sums

Allowances that may change later; flag these as potential risk.

### Hidden costs

Items likely to increase the final price (e.g., site works, rock removal).

### Scope gaps

Missing or unclear items that require clarification.

---

## Safety

- Do not guess prices or fabricate missing details.  
- Do not provide legal, financial, or contractual advice.  
- If the quote is incomplete or unclear, state this explicitly

---
