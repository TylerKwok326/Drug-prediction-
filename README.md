# Lung Cancer Prognostic Markers and Therapeutic Targets Analysis

## Project Overview
This repository contains comprehensive research on lung adenocarcinoma (LUAD) biomarkers and therapeutic targets, with a specific focus on FABP4. The project combines initial biomarker analysis with subsequent computational drug interaction studies to identify potential therapeutic interventions.

## Research Motivation
- Lung cancer remains one of the leading causes of cancer-related deaths worldwide
- Multiple subtypes exist, including Non-Small Cell Lung Cancer (NSCLC) and Small Cell Lung Cancer (SCLC)
- Lung adenocarcinoma (LUAD) presents unique challenges due to its asymptomatic early stages
- There is an urgent need for improved prognostic markers and therapeutic targets

## Project Components

### 1. Initial Biomarker Analysis
Our initial analysis, presented in the PowerPoint, revealed:
- Comprehensive gene expression profile comparison between early-stage and invasive LUAD
- Identification of 125 overlapping genes and 73 genes unique to metastatic lung cancer
- FABP4's emergence as a significant target through:
  - Functional enrichment analysis (PPI enrichment p-value < 1e-16)
  - Regulatory network analysis showing PPAR gamma and SP1 regulation
  - Evidence supporting FABP4's role in cancer progression

### 2. Computational Drug Analysis

#### Jupyter Notebooks
- `Bioactivity_data.ipynb`: Processing of initial bioactivity data
- `Descriptor_Dataset_Preparation.ipynb`: Preparation of molecular descriptor datasets
- `Exploratory_Data_Analysis.ipynb`: Statistical analysis and data visualization
- `training.ipynb`: Machine learning model development and validation

#### Data Files

**Raw Data:**
- `FABP4_01_bioactivity_data_raw.csv`: Initial bioactivity measurements
- `FABP4_descriptors_rdkit.csv`: RDKit-generated molecular descriptors
- `molecule.smi`: SMILES notation for analyzed molecules

**Processed Data:**
- `FABP4_02_bioactivity_data_preprocessed.csv`: Cleaned bioactivity data
- `FABP4_03_bioactivity_data_curated.csv`: Curated dataset
- `FABP4_04_bioactivity_data_3class_pIC50.csv`: Three-class pIC50 classification
- `FABP4_05_bioactivity_data_2class_pIC50.csv`: Binary pIC50 classification
- `FABP4_06_bioactivity_data_3class_pIC50_rdkit_fp.csv`: Integrated fingerprint data

## Key Findings

### FABP4 as a Therapeutic Target
1. **Pathway Integration**
   - Significant involvement in LUAD progression mechanisms
   - Direct regulation through the PPAR gamma pathway
   - Multiple interaction points with cancer-related pathways

2. **Drug Interaction Analysis**
   - Valproic acid demonstrated significant interaction with FABP4-related pathways
   - Several approved drugs showed potential for repurposing
   - Integration with known cancer pathways suggests synergistic therapeutic approaches

### Machine Learning Model Results
1. **Model Performance**
   - Random Forest Regressor achieved R-squared score: 0.5926 on test set
   - Model trained on molecular fingerprint features (2048 dimensions)
   - 80/20 train-test split with random state control
   - Variance threshold feature selection (threshold = 0.8 * (1 - 0.8))
   - Clear positive correlation between experimental and predicted pIC50 values

2. **Dataset Characteristics**
   - Input features: Binary molecular fingerprints (fp_0 to fp_2047)
   - Target variable: pIC50 (float64)
   - Dataset size: 2059 compounds
   - Feature types: int64 for fingerprints, float64 for pIC50

### Drug Analysis Results
1. **Primary Drug Candidates**
   - Valproic acid emerged as a leading candidate
   - Multiple FDA-approved drugs showed promising FABP4 pathway interactions

2. **Pathway Analysis**
   - Identified key interaction nodes in the FABP4 pathway
   - Mapped drug effects on downstream signaling
   - Validated through computational modeling and statistical analysis

## Future Directions
1. Experimental validation of computational predictions
2. Investigation of drug combination strategies
3. Development of FABP4-targeted therapeutic approaches
4. Extension of analysis to other lung cancer subtypes

