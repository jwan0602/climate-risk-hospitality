# Climate Risk and IT Investment Impact on Hotel Performance

## Overview

This project investigates how climate risk influences hotel financial performance and how information technology (IT) investments mitigate operational risk under uncertain environmental conditions.

Hospitality businesses operate in geographically distributed environments where climate-related disruptions can significantly affect revenue stability. This project integrates large-scale hotel performance data with regional climate risk indicators to quantify how technology investments enhance resilience.

Using panel data modeling with mixed-effects regression, this project evaluates how IT spending interacts with climate risk to influence hotel-level revenue performance.

---

## Project Objectives

The primary objectives of this project include:

- Integrate multi-source datasets into a unified panel dataset  
- Construct climate risk indicators from environmental event data  
- Model hotel financial performance under risk conditions  
- Quantify the interaction effect between IT investment and climate risk  
- Generate interpretable insights for operational resilience planning  

---

## Data Sources

This project integrates multiple structured datasets.

### Hotel Performance Data (CBRE)

Property-level hotel performance data including:

- RevPAR (Revenue Per Available Room)  
- IT spending  
- Property identifiers  
- Hotel segment classifications  
- Annual performance indicators  

This dataset captures operational performance across multiple years.

---

### Climate Risk Data (NOAA)

Climate risk indicators derived from:

- Weather events  
- Environmental damage records  
- Regional climate classifications  

Climate risk variables were constructed using:

- Event frequency  
- Economic damage levels  

These variables were standardized to create interpretable risk scores.

---

### Geographic Mapping

ZIP code-level mapping was used to:

- Match hotel locations to regional climate zones  
- Align operational data with environmental conditions  

This step ensured accurate spatial linkage across datasets.

---

## Data Integration Workflow


Hotel Performance Data (CBRE)
↓
ZIP Code Mapping
↓
Climate Risk Data (NOAA)
↓
Regional Alignment
↓
Panel Dataset Construction
↓
Mixed-Effects Regression Modeling


---

## Methods

This project applies advanced panel data modeling to estimate operational impacts under environmental uncertainty.

---

### Step 1 — Climate Risk Construction

Climate risk indicators were constructed using:

- Event counts  
- Damage values  

Transformations included:

- Log transformations  
- Principal Component Analysis (PCA)  
- Standardization (z-score normalization)

This produced interpretable composite climate risk scores.

---

### Step 2 — Panel Data Preparation

Hotel-level panel datasets were structured using:

- Property identifier (panel unit)  
- Year (time dimension)  

Data preprocessing included:

- Missing value handling  
- Variable transformation  
- Lagged variable construction  
- Within–between variable decomposition  

These steps ensured reliable model estimation.

---

### Step 3 — Mixed-Effects Regression Modeling

Primary modeling approach:

**Mixed Linear Model (MixedLM)**

Dependent variable:

- Log-transformed RevPAR (revpar_log)

Key predictors:

- IT investment variables  
- Climate risk indicators  
- Interaction terms (IT × Risk)

Model specification included:

- Random intercepts at property level  
- Random slopes for IT investment  
- Fixed effects for time and region  

This approach captures both:

- Cross-property variation  
- Within-property temporal changes  

---

### Step 4 — Model Evaluation

Model diagnostics included:

- Random-effects evaluation  
- Variance decomposition  
- Model fit comparison  
- Robustness checks  

These ensured statistical reliability of results.

---

## Example Workflow

Raw Hotel Data
↓
Climate Risk Construction
↓
Geographic Mapping
↓
Panel Dataset Creation
↓
Mixed-Effects Modeling
↓
Performance Impact Interpretation


---

## Key Findings

This project identified several meaningful operational patterns.

---

### IT Investment as a Risk Mitigation Tool

Hotels increasing IT spending during high-risk periods demonstrated improved revenue performance relative to peers.

This suggests:

Technology investment functions as a resilience mechanism under uncertain environmental conditions.

---

### Interaction Effects Matter

The interaction between IT investment and climate risk revealed:

IT investments were more valuable under high-risk conditions than under stable conditions.

This finding highlights the strategic importance of adaptive technology investment planning.

---

### Property-Level Variability

Significant variation was observed across individual properties.

Random-effects modeling showed:

Some hotels benefited more from IT investment depending on regional risk exposure.

This supports location-sensitive strategy development.

---

## Business Applications

This framework supports data-driven decision-making in operational strategy and risk management.

Potential applications include:

- Climate risk planning  
- Infrastructure investment strategy  
- Operational resilience modeling  
- Financial performance forecasting  
- Risk-adjusted capital allocation  

Industries that can apply this approach include:

- Hospitality  
- Real estate  
- Insurance  
- Infrastructure management  
- Travel platforms  

---

## Example Outputs

Typical outputs generated include:

- Risk-adjusted performance models  
- Regional risk comparison tables  
- IT investment impact estimates  
- Revenue resilience analysis  
- Model diagnostic reports  

These outputs enable strategic planning under uncertainty.

---

## Technical Skills Demonstrated

This project demonstrates applied expertise in:

- Panel Data Modeling  
- Mixed-Effects Regression  
- Risk Analytics  
- Time-Series Integration  
- Geographic Data Mapping  
- Statistical Modeling  
- Performance Forecasting  

---

## Tools and Libraries

Primary tools used:

- Python  
- pandas  
- numpy  
- statsmodels  
- scikit-learn  
- matplotlib  

These tools enabled scalable statistical analysis and model estimation.

---

## Reproducibility

This repository includes:

- Data preparation scripts  
- Model specification notebooks  
- Example regression outputs  

The workflow is modular and adaptable to other panel datasets.

---

## Author

Jaewan Heo  
Ph.D. Candidate — Hospitality Analytics  
Panel Modeling | Risk Analytics | Applied Econometrics
