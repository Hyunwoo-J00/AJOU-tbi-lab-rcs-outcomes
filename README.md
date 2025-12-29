# TBI Laboratory Variables and Outcomes  
### Restricted Cubic Spline (RCS) Analysis

This repository summarizes an exploratory study that examines the association between **early routine laboratory variables** and **traumatic brain injury (TBI) outcomes**, using **restricted cubic spline (RCS) logistic regression**.

The purpose of this work is to organize and visualize non-linear relationships between laboratory measurements obtained at admission and short- and long-term outcomes after TBI.

---

## Study Design

### Study population
Patients were selected from a cohort of TBI patients treated at **Ajou University Hospital**.

Inclusion criteria:
- Arrival within **12 hours after injury**
- **Head/Neck AIS ≥ 3**

From the eligible population, two analysis cohorts were defined based on outcome availability and complete laboratory data:
- **14-day mortality cohort**
- **6-month outcome cohort**, defined by Glasgow Outcome Scale–Extended (GOSE)

---

## Outcomes

Two outcomes were analyzed in parallel:

1. **14-day mortality**  
   (death vs survival)

2. **6-month unfavorable outcome**  
   (GOSE 1–4 vs 5–8)

---

## Laboratory Variables

A total of **25 routine laboratory variables** measured at admission were included.

### Primary panel
Eight laboratory variables were predefined as clinically core markers:

- Glucose  
- CRP  
- Hemoglobin  
- Albumin  
- Creatinine  
- Platelet count  
- INR  
- Sodium  

### Secondary panel
The remaining laboratory variables were grouped by physiological systems:

- **Liver function / tissue injury**  
  AST, ALT, ALP, total bilirubin, total protein, total cholesterol

- **Renal function / nitrogen metabolism**  
  BUN, uric acid

- **Electrolytes / acid–base balance**  
  Potassium, calcium, chloride, total CO₂

- **Inflammation / cell counts**  
  White blood cell count

- **Muscle / myocardial enzymes**  
  Creatine kinase, CK-MB

---

## Statistical Analysis

To evaluate potential **non-linear associations** between laboratory variables and outcomes, we applied:

- **Logistic regression with restricted cubic splines (RCS)**

Analyses were conducted in two stages:
- **Univariable RCS models**
- **Multivariable RCS models**, adjusted for:
  - Age  
  - Glasgow Coma Scale (GCS) score  
  - Head/Neck AIS  
  - Pupil reactivity  
  - Epidural hemorrhage  
  - Subarachnoid hemorrhage  

Odds ratios are referenced to the **median value** of each laboratory variable.

---

## Visualization

This repository provides **interactive RCS odds ratio plots** for each laboratory variable and outcome.

Each plot displays:
- The estimated odds ratio curve
- 95% confidence intervals
- The median reference point

Plots are organized by laboratory panels, and each laboratory variable can be explored for both outcomes.

---

## Purpose of This Repository

This repository is intended to:
- Share the overall **analysis framework**
- Provide **interactive visualization** of RCS results
- Facilitate discussion on study direction and interpretation

It is not intended to present finalized results or clinical recommendations.

---

**Hyunwoo Jeon**  
Ajou University School of Medicine

