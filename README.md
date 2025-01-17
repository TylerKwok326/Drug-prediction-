# Drug-prediction-
Lung Cancer Prognostic Markers and Therapeutic Targets Analysis

Project Overview
This repository documents our investigation into lung adenocarcinoma (LUAD) biomarkers and therapeutic targets, with a particular focus on FABP4. Our initial analysis presented in the PowerPoint revealed FABP4 as a promising therapeutic target, leading to subsequent computational drug interaction studies.
Research Motivation

Lung cancer remains one of the deadliest diseases worldwide
Multiple subtypes exist, including NSCLC and SCLC
LUAD (lung adenocarcinoma) presents a critical challenge due to asymptomatic early stages
Need for better prognostic markers and therapeutic targets

Project Components
1. Initial Analysis (PowerPoint Presentation)

Analysis of gene expression profiles between early-stage and invasive LUAD
Identification of 125 overlapping genes and 73 genes unique to metastatic lung cancer
Discovery of FABP4's significance through:

Functional enrichment analysis showing PPI enrichment (p-value < 1e-16)
Regulatory network analysis revealing PPAR gamma and SP1 regulation
Evidence of FABP4's role in cancer progression



2. Computational Analysis (Jupyter Notebooks)
Based on the presentation findings highlighting FABP4's importance, we conducted:

Jupyter Notebooks

Bioactivity_data.ipynb: Initial bioactivity data processing
Descriptor_Dataset_Preparation.ipynb: Dataset preparation
Exploratory_Data_Analysis.ipynb: Statistical analysis
training.ipynb: Model development

Data Files
Raw Data

FABP4_01_bioactivity_data_raw.csv
FABP4_descriptors_rdkit.csv
molecule.smi

Processed Data

FABP4_02_bioactivity_data_preprocessed.csv
FABP4_03_bioactivity_data_curated.csv
FABP4_04_bioactivity_data_3class_pIC50.csv
FABP4_05_bioactivity_data_2class_pIC50.csv
FABP4_06_bioactivity_data_3class_pIC50_rdkit_fp.csv

Analysis Results

Statistical analysis files (Mann-Whitney tests)
Visualization plots

Key Findings
1. FABP4 Significance (from Presentation)

Involvement in LUAD progression
Regulation by PPAR gamma pathway
Potential as therapeutic target

2. Drug Analysis Results

Valproic acid shows significant interaction with FABP4-related pathways
Multiple approved drugs show potential for repurposing
Integration with known cancer pathways
