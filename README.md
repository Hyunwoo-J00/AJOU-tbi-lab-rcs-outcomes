# TBI Laboratory Biomarkers and Outcomes  
### Multivariable Restricted Cubic Spline (RCS) Analysis

This repository shares the current analytical results and manuscript outline for a study that aims to **systematically evaluate the association between early routine laboratory variables and traumatic brain injury (TBI) outcomes**, independent of our previously ongoing TBI prognostic model research.

The primary focus of this work is the **non-linear relationship between initial laboratory measurements and TBI outcomes**, assessed using **restricted cubic spline (RCS) logistic regression**, and visualized through interactive odds ratio (OR) plots.

---

## 1. Study Population

From a total of **4,461 TBI patients** treated at **Ajou University Hospital**, the following inclusion criteria were applied:

- Arrival within **12 hours after injury**
- **Head/Neck AIS ≥ 3**

After applying these criteria, **2,728 patients** were included.

### Analysis cohorts
- **14-day mortality cohort**  
  - Outcome available: 2,242 patients  
  - Complete laboratory data: **2,221 patients**

- **6-month outcome cohort (GOSE)**  
  - Outcome available: 2,116 patients  
  - Complete laboratory data: **2,097 patients**

As shown in **Table 3**, baseline characteristics were highly comparable between the full cohort and each analysis cohort, suggesting that **selection bias due to outcome availability or laboratory missingness is likely minimal**.

### Outcomes
Two outcomes were analyzed in parallel:
1. **14-day mortality** (death vs survival)
2. **6-month unfavorable outcome**  
   *(GOSE 1–4 vs 5–8)*  
(see Tables 1–2)

---

## 2. Analysis Overview

### 2.1 Patient characteristics
Patient characteristics stratified by:
- 14-day mortality
- 6-month unfavorable outcome  

were summarized in **Table 1** and **Table 2**, respectively.

- Continuous variables: Welch’s t-test  
- Categorical/ordinal variables: Chi-square test  
- P-values are reported accordingly.

---

### 2.2 Boxplots and outlier handling

For all **25 laboratory variables**, outcome-stratified boxplots were generated to evaluate distributions and extreme values.

To mitigate the influence of extreme outliers:
- Values below the **1st percentile** and above the **99th percentile** were **clipped to the respective percentile values**.
- This strategy was visualized and documented alongside boxplots in a PowerPoint file.

---

### 2.3 Univariable and multivariable RCS logistic regression

To assess **non-linear associations** between laboratory variables and outcomes, we applied **restricted cubic spline (RCS) logistic regression**.

#### Univariable RCS
- Used to explore the overall shape of the association
- Overall spline p-values were evaluated

#### Multivariable RCS
Adjusted for the following covariates:
- Age
- Glasgow Coma Scale (GCS) score
- Head/Neck AIS
- Pupil reactivity
- Epidural hemorrhage
- Subarachnoid hemorrhage

Results are summarized in **Table 4**, presenting unadjusted and adjusted spline p-values in parallel.  
RCS OR plots for each laboratory variable are provided separately for univariable and multivariable models.

---

## 3. Primary vs Secondary Laboratory Panels

### Primary panel
Eight laboratory variables were predefined as the **primary panel**, based on:
- Consistent reporting in prior TBI and critical care prognostic studies
- Variables identified as important in our previous work

Primary panel variables:
- Glucose
- CRP
- Hemoglobin
- Albumin
- Creatinine
- Platelet count
- INR
- Sodium

### Secondary panel
The remaining 17 laboratory variables constitute the **secondary panel**, grouped by physiological systems:

**Liver function / tissue injury**
- AST, ALT, ALP
- Total bilirubin
- Total protein
- Total cholesterol

**Renal function / nitrogen metabolism**
- BUN
- Uric acid

**Electrolytes / acid–base balance**
- Potassium
- Calcium
- Chloride
- Total CO₂

**Inflammation / cell counts**
- White blood cell count (WBC)

**Muscle / myocardial enzymes**
- Creatine kinase
- CK-MB

For the secondary panel, **false discovery rate (FDR)-adjusted q-values** will be additionally calculated and presented as supplementary material to account for multiple testing.

---

## 4. Rationale for Excluding Quartile-based OR and Forest Plots

During exploratory analyses, we initially evaluated:
- ORs comparing the 25th vs 75th percentiles
- ORs comparing central vs extreme percentile ranges

However, inspection of the spline curves revealed that:
- Risk often increases sharply only beyond specific percentiles
- Several variables demonstrate **U-shaped or asymmetric relationships**

As a result, single cut-off–based OR summaries and forest plots were deemed **insufficient to represent the true association patterns** and were excluded from the final analysis.

Instead, this study emphasizes:
- The **shape of the RCS curves**
- Overall spline significance
- Qualitative interpretation of risk patterns

---

## 5. Interpretation Strategy Based on Spline Shapes

Rather than proposing strict cut-offs for all variables, we plan to describe associations qualitatively, for example:

- *“INR shows a marked increase in risk beyond approximately 1.1.”*
- *“Sodium demonstrates increased risk at both hypo- and hypernatremic ranges.”*

These descriptions aim to reflect the **underlying spline-derived risk patterns** more faithfully than dichotomized thresholds.

---

## 6. Significance of the Study

Previous TBI prognostic models (e.g., IMPACT, CRASH) included only a limited number of laboratory variables or none at all.

This study is distinct in that it:
- Evaluates **25 routine laboratory variables**
- Assesses **both short-term mortality and long-term functional outcome**
- Applies **non-linear modeling consistently across all variables**
- Differentiates **clinically core markers (primary panel)** from **broader organ function markers (secondary panel)**
- Incorporates **FDR correction** for exploratory analyses

Overall, this work is positioned as a **structured exploratory analysis**, rather than simple data mining.

---

## 7. Ongoing and Future Directions

Planned additional analyses include:

### Covariate–laboratory relationships
- Exploring associations between age and selected labs (e.g., glucose, creatinine, CRP)
- Evaluating differences in laboratory distributions by GCS strata
- Providing supplementary figures to contextualize attenuation of lab effects after adjustment

### Spline-based qualitative interpretation
- Refining narrative descriptions of spline shapes for the manuscript text

### Future projects
This laboratory-focused manuscript is intended as a standalone study. Potential subsequent projects include:
1. Imaging variables and outcomes
2. Comparative analysis of level of consciousness and GCS
3. Machine learning–based enhancement of TBI prognostic models
4. CNN-based models incorporating imaging directly into outcome prediction

---

## 8. Shared Materials

The following files are included or referenced:

- **Tables.docx** – Tables 1–4  
- **Lab_Box_plot.pptx** – Outcome-stratified boxplots and clipping strategy  
- **univariable_OR_plot.pptx** – Univariable RCS OR plots  
- **multivariable_OR_plot.pptx** – Multivariable RCS OR plots  

---

## 9. Notes

This repository is shared to facilitate discussion on:
- Overall study direction
- Analytical completeness
- Interpretation strategy
- Target journal selection (e.g., *Neurosurgery*, *Journal of Neurosurgery*)

Feedback and suggestions are welcome. A manuscript draft will be prepared after incorporating co-author feedback.

---

**Hyunwoo Jeon**  
Ajou University School of Medicine  
