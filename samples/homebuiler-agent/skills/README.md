# Homebuilder agent skills pack

## Overview

The skills pack defines the behavioural, decision‑making and routing logic used by the Homebuilder agent. Skills extend the agent’s capabilities beyond static knowledge by providing structured reasoning patterns, domain‑specific workflows and consistent handling of user requests.

- Skills are not tools
- Tools perform actions
- Skills define how the agent thinks

The skills pack ensures that the agent behaves predictably, safely and consistently across all supported scenarios.

## Purpose

The skills pack provides:

- domain‑specific reasoning patterns
- decision trees for builder verification, quote analysis and site assessment
- routing logic for selecting tools
- structured response formats
- safety and boundary rules
- consistent terminology and phrasing

It ensures that the agent’s behaviour is aligned with Queensland residential construction practice and the Homebuilder knowledge pack.

## Skill categories

### Builder verification skills

These skills define how the agent:

- interprets builder‑related questions
- decides when to call licence, disciplinary or financial tools
- synthesises results into a risk profile
- explains findings using the knowledge pack

### Quote analysis skills

These skills define how the agent:

- interprets quote‑related uploads
- extracts PS/PC items
- identifies red flags
- compares multiple quotes
- explains risks and differences

### Site and overlay assessment skills

These skills define how the agent:

- interprets site‑related questions
- checks overlays
- analyses slope, soil, fill and drainage
- estimates site cost risk
- produces structured site reports

### Covenant and design skills

These skills define how the agent:

- interprets covenant and design documents
- checks compliance
- explains non‑compliant elements
- recommends next steps

### Workflow and briefing skills

These skills define how the agent:

- generates builder briefs
- produces site summaries
- structures outputs for communication with builders or consultants

### Design principles

The skills pack is built on the following principles:

- deterministic behaviour
- strict separation of knowledge, skills and tools
- predictable routing
- no inference of missing parameters
- consistent structure across responses
- alignment with Queensland building practice

## Versioning

The skills pack should be versioned independently from the tools pack and knowledge pack.
Changes should be documented in a CHANGELOG file.
