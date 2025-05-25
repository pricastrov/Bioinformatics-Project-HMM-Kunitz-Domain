# 🧬 Modeling the BPTI/Kunitz Domain: A Profile HMM Approach for Protein Domain Annotation

This project applies a profile Hidden Markov Model (HMM) approach to detect and annotate the BPTI/Kunitz protease inhibitor domain across protein sequences. Through MSA, HMM construction, and sequence scanning, the pipeline enables accurate identification of domain-containing proteins for functional annotation and comparative analysis.

## Summary of the workflow
![Kunitz drawio](https://github.com/user-attachments/assets/5a4a71ba-5e31-4fac-a423-3dc55912d60d)

**Figure 1. Workflow of the project.** The data collection was made from the PDB and the Uniprot/Swiss-Prot websites. The structures were clustered and aligned. The alignment was then visualized. The clusters were used to build a profile HMM that was validated with sets obtained from Uniprot/Swiss-Prot. The validation results were analyzed, and classification metrics were obtained (Diagram made with https://app.diagrams.net).

##
