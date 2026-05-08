# Narrative–Technical Drift Project

This repository contains the implementation work for our ECE 60872 project on applying GitHub bug-fix classifiers to evaluate narrative–technical drift in postmortems.

## Current Contents

- `Phase_1_GitHub_Drift_Scoring.ipynb`  
  A step-by-step annotated Google Colab notebook for Phase 1.

## Phase 1

Phase 1 collects linked GitHub issue–pull request pairs and computes a Narrative–Technical Drift score from:

- narrative severity features from issue/PR text
- technical risk features from patch metadata
- sensitive-file indicators

The notebook is written to be run in Google Colab.

## How to Run

1. Open the notebook in Google Colab.
2. Mount Google Drive when prompted.
3. Add a GitHub token if available, preferably through Colab secrets as `GITHUB_TOKEN`.
4. Run the notebook cells in order.

The notebook is annotated throughout, so each block explains what it is doing and how it contributes to the Phase 1 drift-baseline.

## Status

Only Phase 1 is currently included. Future work may add the Phase 2 postmortem rubric and Phase 3 weakly supervised transfer classifier.
