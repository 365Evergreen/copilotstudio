# Homebuilder knowledge pack

## Overview

The Homebuilder knowledge pack provides structured, retrieval‑ready reference material used by the Homebuilder agent to explain concepts, processes and risks involved in residential construction in Queensland. It contains factual, non‑actionable information that supports the agent’s reasoning and enables it to provide clear, consistent guidance to users.

The knowledge pack does not contain live data, builder‑specific information or regulatory lookups. Instead, it provides the contextual understanding required to interpret tool outputs, explain terminology, and guide users through the homebuilding process.

The pack is designed to be:

- modular  
- retrieval‑friendly  
- chunked into atomic topics  
- aligned with Queensland regulations and building practices  
- neutral, factual and non‑prescriptive  

It complements the tools pack by providing the explanatory layer that tools alone cannot supply.

---

## Structure

The knowledge pack is organised into topic‑specific Markdown files. Each file contains:

- a YAML header for metadata  
- a single topic per file  
- consistent formatting  
- publicly available summaries only  
- no proprietary or copyrighted content  

Topics include:

- QBCC licensing  
- QBCC financial requirements  
- QBCC complaints and disciplinary actions  
- Home warranty insurance  
- Provisional sums and prime cost items  
- Site costs  
- Builder quotes  
- Bushfire zones and BAL ratings  
- Flood zones  
- Overland flow  
- Covenants and design guidelines  
- Planning and building approvals  

Each topic is written to be self‑contained and suitable for retrieval‑augmented generation.

---

## Purpose

The knowledge pack enables the Homebuilder agent to:

- explain building terminology  
- describe regulatory processes  
- outline typical risks and considerations  
- interpret tool outputs in context  
- provide general guidance without giving legal, financial or engineering advice  

It ensures that explanations are consistent, accurate and aligned with Queensland practice.

---

## Usage principles

### When the agent should use the knowledge pack

The agent should rely on the knowledge pack when the user asks for:

- definitions  
- explanations  
- general guidance  
- process overviews  
- contextual understanding  
- interpretation of tool results  
- comparisons of concepts (not builders)  

Examples:

- “What is a provisional sum?”  
- “How does home warranty insurance work in Queensland?”  
- “Why do site costs vary so much?”  
- “What does a BAL rating mean?”  

### When the agent should not use the knowledge pack

The agent must not use the knowledge pack when the user asks for:

- builder‑specific information  
- licence checks  
- disciplinary history  
- financial conditions  
- quote analysis  
- site‑specific assessments  
- covenant compliance checks  

In those cases, the agent must use the appropriate tool.

---

## Design principles

The knowledge pack is built on the following principles:

- **Neutrality**: no endorsements, no builder‑specific claims.  
- **Clarity**: plain language, structured explanations.  
- **Accuracy**: aligned with publicly available Queensland guidance.  
- **Boundaries**: no legal, financial or engineering advice.  
- **Retrievability**: chunked for efficient retrieval.  
- **Consistency**: uniform formatting across all files.  

These principles ensure the agent provides reliable, safe and consistent information.

---

## File format and conventions

All files follow these conventions:

- `.md` extension  
- YAML header with title, filename, version, topic and region  
- no H1 headings below the YAML header  
- blank line after YAML  
- blank line after each header  
- URLs wrapped in angle brackets  
- no emojis  
- no proprietary content  
- no duplication across files  

This ensures compatibility with retrieval systems and avoids formatting issues.

---

## Intended audience

The knowledge pack is intended for:

- homeowners  
- first‑time builders  
- users comparing builders or quotes  
- users assessing site risks  
- users navigating Queensland building processes  

It is not intended for professional builders, engineers or certifiers, although the content is accurate enough to support informed discussions with them.

---

## Versioning

The knowledge pack should be versioned independently from the tools pack.  
Changes to content, structure or metadata should be documented in a CHANGELOG file.

---
