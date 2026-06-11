# AI Drug Discovery Pipeline (Cheminformatics + ML)

## 📌 Overview
This project builds a complete computational drug discovery pipeline using RDKit, Machine Learning, and molecular similarity analysis.

It processes a full dataset of 1128 molecules and performs:
- Data cleaning
- Molecular descriptor generation
- Drug-likeness filtering (Lipinski Rule of Five)
- QSAR modeling (solubility prediction)
- Molecular similarity search
- Lead compound ranking system

---

## ⚙️ Dataset
- Source: ESOL solubility dataset
- Total molecules: 1128
- Type: Small organic molecules
- Columns include:
  - SMILES
  - Molecular weight
  - LogP
  - TPSA
  - Experimental solubility

---

## 🧪 Workflow

### 1. Data Processing
- SMILES validation using RDKit
- Conversion to molecular objects

### 2. Feature Engineering
- Molecular descriptors:
  - Molecular Weight
  - LogP
  - TPSA
  - HBD
  - HBA
  - Rotatable Bonds
  - Aromatic Rings

### 3. Drug-Likeness Filtering
- Lipinski Rule of Five:
  - MW ≤ 500
  - LogP ≤ 5
  - HBD ≤ 5
  - HBA ≤ 10

### 4. Machine Learning Model (QSAR)
- Model: Random Forest Regressor
- Target: ESOL solubility
- Performance:
  - R² Score: 0.88
  - RMSE: 0.70

### 5. Similarity Search
- Morgan Fingerprints (RDKit)
- Tanimoto similarity scoring
- Identifies structurally similar compounds

### 6. Lead Scoring System
Final Score = combination of:
- Drug-likeness score
- ML predicted solubility
- Structural similarity

---

## 📊 Results

- Total molecules processed: 1128
- Drug-like molecules: 1018
- Best QSAR performance: R² = 0.88
- Final ranked drug candidates generated

Top candidates include:
- small organic molecules
- alcohols
- hydrocarbon derivatives

---

## 🚀 Technologies Used
- Python
- RDKit
- Pandas
- Scikit-learn
- NumPy
- Matplotlib

---

## 🧠 Key Concepts Demonstrated
- Cheminformatics
- Molecular descriptors
- QSAR modeling
- Drug-likeness rules
- Fingerprint similarity
- Machine learning regression

---

## 📌 Project Outcome
A complete end-to-end AI-driven drug discovery workflow that simulates early-stage pharmaceutical screening.

---

## 👤 Author
Built as part of a cheminformatics + AI drug discovery learning roadmap.
