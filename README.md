# Narrative–Technical Drift Project

This repository contains the implementation for our ECE 60872 project on applying GitHub bug-fix classifiers to evaluate Narrative–Technical Drift in postmortems.

## Contents

The project is organized into three annotated Google Colab notebooks:

- `Phase_1_GitHub_Drift_Scoring.ipynb`  
  Collects linked GitHub issue–pull request pairs and computes Narrative–Technical Drift scores.

- `Phase_2_Postmortem_Accountability_Labeling.ipynb`  
  Applies the postmortem accountability rubric and organizes human/LLM scoring.

- `Phase_3_Weakly_Supervised_Transfer.ipynb`  
  Trains a weakly supervised embedding-based classifier using GitHub drift labels and applies it to postmortem text.

## How to Run

1. Open each notebook in Google Colab.
2. Mount Google Drive when prompted.
3. Add any required input files to the expected Drive folder.
4. Run the notebook blocks in order.

Each notebook is step-by-step annotated, so the blocks explain what they do and how they connect to the overall pipeline.

## Pipeline Summary

Phase 1 builds the GitHub-derived drift-baseline.  
Phase 2 creates accountability scores for postmortems.  
Phase 3 compares the GitHub-derived drift signal against the postmortem accountability scores.

## Notes

The notebooks are designed for reproducibility in Google Colab. A GitHub token can be added through Colab secrets as `GITHUB_TOKEN` to improve API access during Phase 1.
