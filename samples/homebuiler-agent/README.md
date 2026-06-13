# Homebuilder agent

## Overview

The Homebuilder agent is a domain‑specific conversational assistant designed to help users understand builder quotes, site conditions, regulatory requirements and construction risks in Queensland. It combines three layers:

- Knowledge pack: factual, explanatory content
- Skills pack: reasoning and decision‑making logic
- Tools pack: operational capabilities for real‑world lookups and document analysis

Together, these layers enable the agent to provide structured, accurate and practical guidance throughout the early stages of the homebuilding process.

## Repository structure

A recommended structure is:

Code
/agent
  /knowledge
    qld-qbcc-licensing.md
    qld-qbcc-financials.md
    ...
  /skills
    builder-verification.md
    quote-analysis.md
    site-assessment.md
    ...
  /tools
    schema.json
    README.skills.md
    README.tools.md
  agent-system-prompt.md
  agent-routing-rules.md
  README.md

This structure separates concerns and simplifies maintenance.

## Components

### Knowledge pack

Contains topic‑specific Markdown files covering:

- QBCC licensing
- financial requirements
- disciplinary actions
- home warranty insurance
- provisional sums and prime cost items
- site costs
- overlays
- covenants
- planning approvals

The knowledge pack provides context and explanations.

### Skills pack

Defines:

- reasoning patterns
- routing logic
- decision trees
- structured response formats
- safety boundaries

The skills pack determines how the agent behaves.

### Tools pack

Provides operational capabilities:

- builder lookups
- quote analysis
- site assessment
- overlay checks
- covenant compliance
- structured report generation

The tools pack enables the agent to perform actions.

## Editing the agent

The agent is edited through:

- System prompt
- Skills
- Knowledge sources
- Tools
- Routing rules

Each layer must be updated independently to avoid unintended behavioural changes.

## Development workflow

1. Update knowledge files as needed
2. Update skills when behaviour must change
3. Update tools when new capabilities are required.
4. Update the system prompt to wire everything together.
5. Test using the testing matrix.
6. Commit changes with clear versioning.

## Testing matrix

A testing matrix is included in the repository to validate:

- tool routing
- parameter extraction
- knowledge usage
- skill behaviour
- error handling

## Visual Studio Code

### Guide

This guide explains how to edit the Homebuilder agent using Visual Studio Code. It covers file organisation, editing workflows and recommended extensions.

#### Prerequisites

- Visual Studio Code installed
- Git repository cloned locally
- Markdown support enabled (built‑in)

#### Folder structure

Ensure the repository follows a clear structure:

Code
/agent
  /knowledge
  /skills
  /tools
  agent-system-prompt.md
  agent-routing-rules.md

This allows VS Code to provide clean navigation and search.

#### Editing knowledge files

Knowledge files are plain Markdown.

When editing:

- keep the YAML header intact
- maintain one topic per file
- avoid duplication
- use sentence case
- wrap URLs in angle brackets
- avoid emojis
- ensure headings follow the established pattern
- Use the Markdown preview (Ctrl+Shift+V) to verify formatting.

#### Editing skills

Skills define reasoning behaviour.

When editing:

- maintain consistent structure
- avoid tool‑specific logic inside skills
- ensure skills reference knowledge topics correctly
- avoid circular reasoning
- keep decision trees explicit

Skills should be edited cautiously, as they directly affect agent behaviour.

#### Editing tools

Tools are defined in JSON or YAML schemas.

When editing:

- validate JSON using VS Code’s built‑in validator
- ensure field names match tool definitions in Copilot Studio
- avoid renaming fields without updating the agent system prompt
- keep input and output structures stable

Breaking tool schemas will break the agent.

#### Editing the system prompt

The system prompt wires together:

- knowledge
- skills
- tools
- routing logic

When editing:

- avoid removing behavioural rules
- ensure tool invocation rules remain consistent
- keep the tone and boundaries intact
- update references when adding new tools or skills

The system prompt is the most sensitive file in the project.

#### Editing routing rules

Routing rules determine when the agent uses:

- knowledge
- skills
- tools

When editing:

- ensure rules are mutually exclusive
- avoid ambiguous conditions
- test each scenario using the testing matrix

## Testing changes

Use the testing matrix to validate:

- tool selection
- parameter extraction
- knowledge usage
- skill behaviour
- error handling

Testing should be performed after every significant change.

## Version control

Commit changes with clear messages, for example:

feat: add bushfire overlay knowledge file
fix: correct PS/PC extraction logic
refactor: restructure builder verification skills
docs: update system prompt and routing rules
Tag releases when major behavioural changes occur
