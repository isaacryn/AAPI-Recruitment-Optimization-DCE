# AAPI-Recruitment-Optimization-DCE

# Optimizing AAPI Recruitment for Alzheimer's Research: A Discrete Choice Experiment (DCE)

**Author:** Isaac Nguyen
**Status:** Completed

---

##  Executive Summary

This is an independent Collab Project on DCE Simulation + Demographic Weighting for AANHPI Recruitment

Note:
Since I can't access private patient data, I'm generating synthetic dataa that statistically mirrors the reported Odds Ratios to understand the underlying probability distributions modeled in the Paper.

Summary: My Goal was to create a data set that mimics the structure of the CARE registry survey, create a mock dataset of 1000 AANHPI seniors that replicates the specific utility weight
(preferences found in the study, including the unique deviations for Vietnamese participants)By statistically replicating the study's Discrete Choice Experiment, using Monte Carlo simulations,
this notebook identifies high yield recruiement channels for underrepresented AAPI subgroups.
My analysis extends the proof that a "one size fits all" digital strategy fails for specific demographics, and as a vietnamese american, I chose to focus on Vietnamese seniors and
I provided a theoretical segmented budget that could maximize recruitment ROI.

A DCE dataset requires a 'long format' where each choice task has two rows (Option A and Option B)


## Technical Approach:
This project demonstrates the following data science competencies:
- Uses a Monte Carlo Simulation: Generated a synthetic dataset mirroring the specific probability distributions and utility weights derived from the original literature.
- Behavioral Modeling: Implemented Conditional Logistic Regression using the "Difference Method" to isolate preference utilities for recruitment attributes (Who, Why, How).
- Heterogeneity Analysis: Statistically isolated subgroup deviations, specifically quantifying the preference for "Ethnic Radio/TV" among Vietnamese participants (OR > 1.0) vs. other groups.
- Business ROI Modeling: Translated statistical odds ratios into a predictive "Recruitment Yield" calculator to guide budget allocation.

##  Key Findings
1.  **Digital Divide:** While Social Media is the dominant channel for younger demographics (OR: 1.50), it underperforms for specific older subgroups.
2.  **The "Hidden" Channel:** Vietnamese participants showed a statistically significant preference for Ethnic Radio/TV.
3.  **Strategic Recommendation:** A segmented campaign allocating specific resources to radio for Vietnamese targets is projected to increase recruitment yield by **~XX%** (see model outputs) compared to a generic flyer campaign.

## 💻 How to Run This Code
This project is written in Python and designed to run in a Jupyter Notebook environment (Google Colab or Kaggle).

### Dependencies
* `numpy` & `pandas`: Data manipulation and synthetic generation.
* `statsmodels`: Advanced statistical modeling (Conditional Logit).
* `matplotlib` & `seaborn`: Visualization of forest plots and ROI heatmaps.

### Quick Start
1.  Clone this repository.
2.  Install requirements: `pip install pandas numpy statsmodels seaborn`
3.  Run the notebook `AAPI_Recruitment_Optimization.ipynb` sequentially.

## Reference Literature
**Original Study:** Ta Park, V. M., et al. (2023). [cite_start]*Asian Americans' and Pacific Islanders' preferences in recruitment strategies and messaging for participation in the CARE registry: A discrete choice experiment.* Alzheimer's & Dementia, 19, 5198–5208. [cite: 7, 30]

---
*This analysis was conducted as an independent replication to demonstrate statistical modeling and recruitment optimization techniques.*
