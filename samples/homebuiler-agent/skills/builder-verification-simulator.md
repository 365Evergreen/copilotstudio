---
title: Builder Verification Simulator
filename: builder-verification-simulator.md
version: 1.0
skill_type: pseudo-tool
description: Simulated builder verification logic using trust-signal categories for the Homebuilder Copilot.
---


## Purpose

Simulate builder verification using trust‑signal categories without fabricating real‑world data.  
This enables the Homebuilder Copilot to provide structured, consistent builder assessments during the PoC.

---

## Behaviour

When the user asks about a builder:

- Extract the builder name from the user’s message.  
- Use the defined trust‑signal categories to structure the response.  
- If any information is unknown, return **“Not available”**.  
- Provide a simulated score only when clearly marked as **simulated**.  
- Explain what each trust signal represents so the user understands the assessment.  
- Never fabricate real‑world verification data.  

---

## Output Format

Use the following structured format for all builder verification summaries:

### **Builder Verification Summary**

- **Licence status:**  
- **Financial health:**  
- **Complaint history:**  
- **Consumer reviews:**  
- **Industry memberships:**  
- **Homebuilder Score (simulated):**  
- **Notes:**  

---

## Trust Signal Definitions

### Licence status

Indicates whether the builder holds an active licence and whether any restrictions or conditions apply.

### Financial health

Represents general financial stability indicators such as credit behaviour or risk level.

### Complaint history

Summarises any known disputes, complaints, or disciplinary actions.

### Consumer reviews

Reflects aggregated sentiment from review platforms.

### Industry memberships

Includes associations such as HIA or MBA.

---

## Safety

- Never fabricate real‑world builder data.  
- If the user requests real verification, clarify that this is a **simulation** for demonstration purposes.  
- Do not provide legal, financial, or contractual advice.  
