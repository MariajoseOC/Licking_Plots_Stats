Licking_Plots_Stats

This repository contains the Python scripts used for behavioral analysis, licking microstructure quantification, statistical testing, and figure generation for the manuscript on sugar preference and consummatory behavior in rats.

🧪 Overview

This project provides the full analysis pipeline for:

preprocessing raw lickometer data

computing preference ratios

parsing licking microstructure (bursts, inter-lick intervals)

performing statistical analyses (ANOVA, Kruskal–Wallis, post hoc tests)

generating all figures presented in the manuscript

📦 Repository Contents

data/ (if included) – raw and/or processed data files

scripts/ – Python scripts for analysis and plotting

results/ – output figures and summary tables

notebooks/ (optional) – Jupyter notebooks illustrating step-by-step analysis

requirements.txt – Python package dependencies

🚀 Getting Started
1. Clone the repository
git clone https://github.com/MariajoseOC/Licking_Plots_Stats.git
cd Licking_Plots_Stats

2. Install dependencies

Install required Python packages:

pip install -r requirements.txt


(Typical packages include numpy, pandas, matplotlib, scipy, etc.)

🖥 Running Analyses

Scripts are structured so that:

preprocess_data.py – loads and formats raw lick data

microstructure_analysis.py – computes bursts and ILI features

stats.py – performs statistical tests

plot_figures.py – generates plots for manuscript figures

Each script includes comments and function docstrings explaining inputs and outputs.

📄 Usage Example
python preprocess_data.py --input data/raw/ --output data/processed/
python microstructure_analysis.py --data data/processed/ --out results/microstructure/
python stats.py --data data/processed/ --out results/stats/
python plot_figures.py --results results/

📌 Notes / Definitions

Bursts: sequences of licks where ILIs < 250 ms, separated by ILIs > 500 ms

Session length: 30 min two-bottle choice

Groups: Control vs Experimental (14-day sucrose exposure) × Sex

💾 Data Availability

Raw data used to generate the results in the manuscript are available from the corresponding author upon request.
