# Clinical Trial Matching Agent

AI agent that retrieves, evaluates, and ranks clinical trials based on patient eligibility criteria.

---

## Overview

This project connects patient profiles with relevant clinical trials by:

- 🔎 Retrieving trials from ClinicalTrials.gov
- ✅ Evaluating eligibility criteria (met / not met / not enough info)
- 📊 Ranking trials based on relevance and eligibility
- ❓ Identifying missing patient information
- 📄 Generating structured summaries for medical review

---

## Problem

Clinical trial recruitment is inefficient:

- Many eligible patients never find suitable trials
- Physicians cannot manually review thousands of studies

👉 This project automates the matching process using structured reasoning.

---

## How It Works

Pipeline:

1. **Retrieval**  
   Query clinical trials based on patient condition

2. **Eligibility Matching**  
   Parse and evaluate inclusion/exclusion criteria

3. **Scoring & Ranking**  
   Prioritize trials based on:
   - number of matched criteria
   - trial phase
   - recruitment status

4. **Missing Information Detection**  
   Generate questions for unresolved criteria

5. **Output Generation**  
   Structured report per trial

---

## 🧑‍⚕️ Example Input

```json
{
  "age": 55,
  "condition": "breast cancer",
  "smoker": false
}
```
