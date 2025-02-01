
# MScThesis-EarlyDementiaDetection

## About
This repository contains the code for my MSc thesis, titled  **AI-Driven Multimodal Approach for Early Detection and Prevention of Dementia**. This study leverages the Aiginition Longitudinal Biomarker Investigation of Neurodegeneration (ALBION) dataset and focuses on the early detection of dementia (MCI) and deepens our understanding of the risk factors involved. We proposed two approaches for early dementia detection: 

1. **Always-Measured Model** – The Always-Measured Model is a straightforward approach designed to leverage features consistently recorded across all visits.
2. **Voting-Based Hybrid Model** – The Voting-Based Hybrid model is a more sophisticated approach that leverages the unique characteristics of each visit recorded in the dataset. By training separate models on combinations of sequential visits and aggregating their outputs through a majority voting mechanism, it systematically evaluates the predictive value of adding longitudinal data while capturing complementary information from multiple visits.

The repository is structured to reflect the different stages of the research, from data preparation to experimentation and final model deployment.

## Repository Structure

```
MScThesis-EarlyDementiaDetection/
│-- data_preparation/
│-- experiments/
│-- final_models/
│-- README.md
```

### 1. `data_preparation/`
This folder contains the code used to preprocess the ALBION dataset. The pipeline follows the preprocessing steps detailed in the thesis, including:
- Data cleaning and standardization
- Handling missing values (e.g., MICE imputation)
- The validation of our imputation strategies
- Feature selection and refinement methods used

### 2. `experiments/`
This folder includes the code used to experiment with our modeling approaches. Key components:
- Experiments to identify the best models for both approaches:
  - Selection of the best Always-Measured Model
  - Selection of the best individual models for the ensemble 
- Progression analysis

### 3. `final_models/`
This folder contains the best-performing models identified during experimentation. It includes:
- Final selected models for both the Always-Measured and Voting-Based Hybrid approaches
- ExplainerHub, which hosts interactive explainer dashboards for the individual models of the ensemble
- The final ensemble model and its evaluation




