# Homebuilder agent tools pack

## Overview

The tools pack provides a structured set of capabilities used by the Homebuilder Copilot to analyse builders, quotes, sites, covenants and risks within the Queensland residential construction context. The tools are designed to work together, enabling the agent to perform real‑world lookups, extract structured information from documents, and generate actionable outputs for users.

This pack forms the operational layer of the Copilot. It complements the knowledge pack by enabling the agent to perform tasks that require data retrieval, document analysis, or structured generation.

The tools are grouped into four functional domains:

- Builder verification  
- Quote analysis  
- Site and risk assessment  
- User workflow and reporting  

Each tool has a clear purpose, defined inputs and outputs, and predictable behaviour.

---

## Tool categories

### Builder verification tools

These tools retrieve authoritative information about builders from public registers and regulatory sources.

- `lookup_qbcc_licence`  
- `lookup_qbcc_disciplinary_history`  
- `lookup_qbcc_financial_conditions`  
- `summarise_builder_risk_profile`

They are used when the user asks about a builder’s licence, trustworthiness, history, or financial stability.

---

### Quote analysis tools

These tools extract structured information from builder quotes and identify risks or inconsistencies.

- `analyse_quote_document`  
- `extract_ps_pc_items`  
- `detect_quote_red_flags`  
- `compare_quotes`

They are used when the user uploads one or more quotes or asks for a comparison.

---

### Site and risk assessment tools

These tools analyse site conditions, overlays and engineering implications.

- `analyse_site_conditions`  
- `estimate_site_cost_risk`  
- `check_overlays`  
- `generate_site_report`

They are used when the user provides an address or asks about site risks, overlays, or expected site costs.

---

### Covenant and design tools

These tools assess compliance between estate covenants and proposed designs.

- `assess_covenant_compliance`

They are used when the user uploads design guidelines or architectural plans.

---

### Workflow and briefing tools

These tools generate structured outputs for communication with builders or consultants.

- `generate_builder_brief`  
- `generate_site_report`

They are used when the user requests a formal brief or a consolidated site summary.

---

## Tool invocation principles

The agent must follow these principles when deciding whether to use a tool:

1. Use a tool only when the user’s request cannot be fulfilled using knowledge alone.  
2. Extract parameters strictly from user input or uploaded files.  
3. Ask for clarification if required parameters are missing.  
4. Never guess builder names, addresses or file identifiers.  
5. When invoking a tool, output only the tool call.  
6. After tool execution, summarise the results clearly and accurately.  
7. Never fabricate tool outputs or fields.

---

## When to use tools vs knowledge

**Use tools when:**

- The user asks about a specific builder.  
- The user wants licence, disciplinary or financial information.  
- The user uploads a quote for analysis.  
- The user uploads multiple quotes for comparison.  
- The user asks about a specific address or lot.  
- The user wants a site report or builder brief.  
- The user asks whether a design complies with covenants.

**Use knowledge when:**

- The user asks for explanations or definitions.  
- The user asks for guidance on processes, risks or terminology.  
- The user asks about Queensland building codes, soil classes, site costs, overlays or covenants in general.  
- The user wants help interpreting tool results.

---

## Design principles

The tools pack is built on the following principles:

- Deterministic behaviour  
- Clear separation of concerns  
- Strict parameter validation  
- No hidden inference  
- Consistent output structures  
- Alignment with Queensland regulatory frameworks  
- Compatibility with the knowledge pack  

These principles ensure that the Copilot behaves predictably and produces reliable, auditable outputs.

---

## Intended usage

The tools pack is intended for:

- Builder due diligence  
- Quote comparison and risk detection  
- Site feasibility assessment  
- Covenant compliance checking  
- Structured reporting and briefing  

It is not intended to replace professional engineering, legal advice or regulatory approvals. Instead, it provides users with clarity, structure and early‑stage risk identification.

---

## Versioning

This tools pack should be versioned independently from the knowledge pack.  
Changes to tool schemas, routing logic or behaviour should be documented in a CHANGELOG file.

---
