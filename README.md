# SAR Analyser 🧬
A modern, object-oriented Streamlit application for Structure-Activity Relationship (SAR) analysis in drug discovery. Built with RDKit, this tool provides a point-and-click interface for common cheminformatics workflows, eliminating the need to write repetitive Jupyter notebooks for each project.

## 🎯 Overview
SAR Analyser transforms molecular data analysis from a coding task into an interactive experience. Whether you're analyzing scaffolds, clustering compounds, or predicting ADMET properties, this application provides professional-grade tools through an intuitive web interface.

Built for: Medicinal chemists, computational chemists, and drug discovery scientists who want to focus on insights rather than code.

## ✨ Key Features
### 🧪 Chemical Sketcher
- Interactive molecule drawing with Ketcher
- Draw structures directly in the browser
- Export in various formats for analysis

### 📊 DataFrame Wizard
- Upload CSV files with molecular data
- Automatic data cleaning and validation
- Statistical summaries and visualizations
- Multiple plot types (histograms, scatter, heatmaps, box plots)
- Molecular grid visualization with mols2grid
- Calculate molecular descriptors on-the-fly
- ADMET Predictions: Built-in admetica integration for predicting:
    - Absorption: Caco-2, Solubility, Lipophilicity, P-gp interactions
    - Metabolism: CYP enzyme substrates and inhibitors (1A2, 2C9, 2C19, 2D6, 3A4)
    - Toxicity: hERG cardiac toxicity, LD50 acute toxicity

### 🔬 Scaffold Hunter
- Murcko scaffold identification
- Scaffold frequency analysis
- Activity distribution per scaffold
- Interactive molecular displays

### 🔍 SMILES Analysis
- Individual molecule deep-dive
- 2D structure visualization
- Comprehensive property calculation: Molecular weight, LogP, TPSA, rotatable bonds, H-bond donors/acceptors, aromatic rings
- Drug-likeness rules (Lipinski, Veber), QED (Quantitative Estimate of Drug-likeness), SA Score (Synthetic Accessibility)
- ADMET properties: solubility, Caco-2 permeability, P-glycoprotein Inhibition, etc
- BRICS fragmentation

### 🎯 R-group analysis
- Clustering using Tanimoto similarity in fingerprints
- Configurable fingerprint types
- Cluster visualization
- Representative molecule selection
- R-group decomposition for each cluster, into their core and attached R-groups
- Frequency of each R-group and representation using tables

## Installation
### 1. Clone the repository
```
git clone https://github.com/ganesh7shahane/SAR_Analyser.git
cd SAR_Analyser
```
### 2. Install dependencies
```
conda env create -f environment.yaml
conda activate streamlit
```
### 3. Run the application
```
streamlit run app.py
```