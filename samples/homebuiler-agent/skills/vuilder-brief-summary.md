---
title: Builder‑Ready Brief Generator
filename: builder-brief-generator.md
version: 1.0
skill_type: pseudo-tool
description: Generates a structured Builder‑Ready Brief from user-provided build details for the Homebuilder Copilot.
---

## Purpose

Generate a structured Builder‑Ready Brief from user‑provided land, budget, build requirements, and site conditions.  
This brief standardises information so builders can quote consistently and users can compare quotes fairly.

---

## Behaviour

When the user provides build details:

- Ask one question at a time  
- Normalise terminology (e.g., “4 bed” → “4 bedrooms”)  
- Accept optional uploads such as land contracts or disclosure plans  
- Fill missing fields with **“Not provided”**  
- Generate the brief once enough information is collected  
- Do not infer details the user has not given  

---

## Output Format

Use the following structured format for all Builder‑Ready Briefs:

### Builder‑Ready Brief

**Land**  

- Suburb:  
- Block size:  
- Land contract uploaded: Yes/No  

**Build**  

- Home style:  
- Bedrooms:  
- Bathrooms:  
- Key inclusions:  
- Special requirements:  

**Budget**  

- Estimated budget:  
- Notes:  

**Site Conditions**  

- Slope:  
- Soil type:  
- Easements:  
- Services:  

**Summary**  

- Key priorities:  
- Risks or unknowns:  

---

## Field Definitions

### Land

Basic property information required for builders to assess suitability and site costs.

### Build

The user’s desired home configuration, inclusions, and any special requirements.

### Budget

The user’s estimated build budget and any relevant constraints.

### Site Conditions

Factors that may affect engineering, slab design, or site works.

### Summary

A concise overview of what matters most to the user and any missing or uncertain details.

---

## Safety

- Do not request sensitive personal information.  
- Do not infer or fabricate details.  
- Do not provide legal, financial, or contractual advice.  
