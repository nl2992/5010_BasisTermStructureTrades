# MATH5010 Final Project — Term Structure Strategies (S1 & S2)

## Overview
This repo contains the final, reproducible notebooks for the MATH5010 project on term-structure trading strategies applied to Bitcoin and commodity futures.

- **S1 (Spot–Futures Basis Capture):** fully-funded spot + short futures package with DTE-based stitching for mark-to-market.
- **S2 (Calendar Spread Mean Reversion):** calendar spread signal and roll-aware execution rules (see S2 notebook for exact spec).

The notebooks build aligned price + DTE panels, compute basis (simple and annualised), run backtests (IS/OOS/FULL), and generate PPT-ready charts (equity curves, VaR/ES histograms, term structure snapshots, regime plots, correlations vs benchmarks).

## What’s in this repo
Everything needed to reproduce our results:
- `S1_FINALBacktest_Submission.ipynb`
- `S2_FINALBacktest_Submission.ipynb`
- `Basis Data.xlsx` (Gold/Silver spot + futures)
- `IBIT.xlsx` (BTC spot (XBT) + BTC futures)
- `5010_final_project.yml` (Conda environment for reproducibility)
- `Math 5010 Project - Final.pdf` (final written report)
- `MATH5010-Prez.pdf` (final presentation slides)

## How to run (end-to-end)

0) Prereq
Install Anaconda or Miniconda (Conda is required).

1) Open a terminal and set the working directory
(Do this so the notebooks can find the Excel files via relative paths.)

    cd path/to/5010_BasisTermStructureTrades

2) Create + activate the environment

    conda env create -f 5010_final_project.yml
    conda activate 5010_final_project

3) Start Jupyter (pick one)

Option A: Classic Notebook (fine if you don’t use Lab)

    jupyter notebook

Option B: JupyterLab

    jupyter lab

Option C: Anaconda Navigator
- Launch “Jupyter Notebook”
- In the file browser, navigate into: 5010_BasisTermStructureTrades

4) Open a notebook and select the kernel
- Open S1_FINALBacktest_submission.ipynb (or S2_FINALBacktest_submission.ipynb)
- Kernel -> Change Kernel -> 5010_final_project

5) Run
Run All (top to bottom).


