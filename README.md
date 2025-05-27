# 🧬 Modeling the BPTI/Kunitz Domain: A Profile HMM Approach for Protein Domain Annotation

## 📄 Table of Contents

- [Overview](#-overview)
- [Repository Structure](#-repository-structure)
- [Objectives](#-objectives)
- [Installation](#-installation)
- [How to Run](#-how-to-run)
- [Results](#-results)
- [References](#-references)
- [Contact](#-contact)

## ‍💻 Overview

This repository contains the code, datasets, and results for a project focused on the identification of the **BPTI/Kunitz domain** using a structure-informed **Profile Hidden Markov Model (HMM)**. The model was constructed from structurally aligned domain sequences and evaluated for domain annotation performance.

## 📁 Repository Structure

Bioinformatics-Project-HMM-Kunitz-Domain/
│
├── data/                       # Input datasets
│   ├── pdb_files_msa/         # PDB files used for MSA
│   ├── preprocessed/          # Cleaned/filtered sequences
│   └── raw/                   # Original downloaded sequences
│
├── docs/                      # Project documentation
│   └── report/                # Final project report (PDF)
│
├── results/                   # Output data
│   ├── evaluation/            # Classification metrics and confusion matrices
│   ├── hmm_profile/           # Final HMM profile
│   └── msa/                   # Multiple sequence and structural alignments
│
├── scripts/                   # Custom Python scripts
│   └── performance.py         # Script to evaluate HMM performance
│
└── README.md                  # This file

## 📌 Objectives

- Construct a profile HMM from structurally aligned Kunitz domain sequences.
- Evaluate its performance on positive and negative datasets using classification metrics.

## 🛠 Installation

Make sure you have the following dependencies installed:

- `Python >= 3.13`
- `BLAST+ >= 2.16.0`
- `CD-HIT >= 4.8.1`
- `HMMER >= 3.4`
- `UCSF Chimera >= 1.20` (optional, for visualization)

## 🚀 Methodology

### 💿 Data preparation (provided in data/)

**1. Retrieve protein sequences from [UniProtKB/Swiss-Prot] (https://www.uniprot.org) with the following criteria:**
  • Taxonomy: _Homo sapiens_ (NCBI Taxonomy ID: 9606)
  • Reviewed: Yes
  • Pfam Domain: PF00014 (Kunitz-type protease inhibitor)

**2. Acquire the [UniProtKB/Swiss-Prot] (https://www.uniprot.org/help/downloads) database file.**

**3. Obtain [PDB structures] (https://www.rcsb.org) with:**
  • Pfam Annotation: PF00014
  • Resolution ≤ 3.5 Å
  • Sequence Length: 45–80 amino acids

**4. Use CD-HIT to cluster sequences based on sequence identity:**

`cd-hit -i pdb_kunitz.fasta -o pdb_kunitz.clst`

### 📏 Multiple Structural Alignment

**1. Upload the IDs of the representatives of the clusters to PDBeFold 

### 🔦 Construction, Validation and Evaluation of the Profile Hidden Markov Model

## 📧 Contact

For questions or feedback, please contact:

### Priscilla Castro-Vargas
Department of Pharmacy and Biotechnology
Alma Mater Studiorum – Università di Bologna
**Email:** priscilla.castro@studio.unibo.it
**ORCID:** 0000-0001-6333-0419

_This project was conducted as part of the Laboratory of Bioinformatics I course at the University of Bologna, 2025._


