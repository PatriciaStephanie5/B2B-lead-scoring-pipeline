# B2B Lead Scoring Pipeline (Python + Pandas)

## Overview
This project simulates a real-world RevOps / Data Analyst task at a B2B company.  
The goal is to prioritize leads for sales outreach using a structured, data-driven scoring model.

---

## Business Problem
Sales teams often waste time on low-quality leads due to lack of prioritization.

This project solves that by:
- identifying high-value prospects
- ranking leads based on business-relevant signals
- enabling more efficient sales outreach

---

## Tech Stack
- Python (Pandas)
- Data Cleaning & Transformation
- Rule-based Lead Scoring Model

---

## Pipeline Architecture

1. Data Ingestion (CSV dataset)
2. Data Cleaning (handling missing values, duplicates)
3. Feature Evaluation:
   - Industry (SaaS = high value)
   - Company Size
   - Engagement Score
4. Lead Scoring Logic
5. Lead Ranking & Segmentation
6. Export (CSV for sales use)

---

## Lead Scoring Model

| Signal | Condition | Score |
|------|----------|------|
| Industry | SaaS | +3 |
| Company Size | >200 employees | +2 |
| Engagement | >70 | +5 |
| Low Engagement | <50 | -2 |

---

## Lead Segmentation

```python
if score >= 8:
    "Hot"
elif score >= 5:
    "Warm"
else:
    "Cold"

**Key Insights**
SaaS companies with high engagement scores consistently ranked as top leads
Larger companies (>200 employees) showed higher prioritization potential
Low engagement leads significantly reduced overall scoring

**Business Impact**
Reduced time spent on low-quality leads
Enabled targeted outreach for high-value prospects
Created a scalable framework for lead qualification.

"*How This Would Be Used in a Company**
- Sales teams receive prioritized lead lists.
- Marketing teams focus nurturing on low-score leads
- Can be integrated into CRM systems for automated scoring


##STAR Framework

**Situation:**
Sales team lacked a structured method to prioritize leads, leading to inefficient outreach.

**Task:**
Develop a scalable lead scoring system to identify high-value prospects.

**Action:**
- Cleaned and processed lead data using Python (Pandas).
- Designed a scoring model based on industry, company size, and engagement.
- Implemented lead ranking and segmentation logic
Result:
- Generated a prioritized list of leads
- Improved sales efficiency by focusing on high-value prospects.
- Created a reusable scoring framework for future campaigns.



