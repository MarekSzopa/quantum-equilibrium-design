# quantum-equilibrium-design
Code and data for the manuscript "Quantum correlations as a resource for equilibrium design in symmetric two-player games"

# Quantum correlations as a resource for equilibrium design

This repository contains the code and source data supporting the manuscript
"Quantum correlations as a resource for equilibrium design in symmetric
two-player games".

## Contents

- `code/Figure1_parameter_regions.nb` – generates Fig. 1.
- `code/Figure2&3_payoff_regions.nb` – generates Fig. 2 and Fig. 3. This .nb requires QEGS.wl
- `code/Figure4_hardware_results.nb` – processes IBM Quantum results and generates Fig. 4. This .nb requires QEGS.wl
- `code/QEGS.wl` - Mathematica package dedicated to investigation of Nash equilibria \
existence in quantum extended games based on EWL scheme
- `code/IBMQ/*.ipynb` – files to create and execute the EWL circuits.
- `data/raw/` – raw IBM Quantum measurement counts. The experiments were performed in June 2026 
### This package was generated from the five raw IBM Quantum count files:
- `wyniki_czysta.txt`
- `wyniki_IIa.txt`
- `wyniki_IiZa.txt`
- `wyniki_iZIa.txt`
- `wyniki_iZiZa.txt`

- `data/processed/` – processed payoff estimates and statistical summaries.
### `data/processed/`
- `Figure4_run_level_payoff_estimates.csv`: all 300 plotted payoff estimates;
- `Figure4_panel_A_payoffs.csv`, `Figure4_panel_B_payoffs.csv`,
  `Figure4_panel_C_payoffs.csv`: panel-specific source data;
- `Supplementary_Table_2_outcome_statistics.csv`;
- `Supplementary_Table_3_payoff_statistics.csv`;
- `Supplementary_Table_4_equal_payoff_precision.csv`.

- `source_data/Source_Data.xlsx` – numerical source data underlying
  the figures and supplementary tables.
### `source_data/Source_Data_Fig4_and_Supplementary_Tables_2-4.xlsx`
A structured workbook containing:
- raw count sheets and derived outcome probabilities;
- reconstructed mixed-strategy distributions;
- the 300 run-level payoff points underlying Fig. 4;
- the statistics reported in Supplementary Tables 2–4.

## Reconstruction of the mixed equilibrium

For every run index, the output probabilities from the four component
circuits `(I,I)`, `(I,iZ)`, `(iZ,I)`, and `(iZ,iZ)` are averaged with
equal weights 1/4. Each component contains 256 shots, so every reconstructed
point is based on 1024 shots in total.

## Scope

This package fully covers Fig. 4 and Supplementary Tables 2–4.
Figures 2 and 3 were generated deterministically in Mathematica. Their exact
numerical source-data exports should be generated from the corresponding
Mathematica notebooks and deposited alongside this package.


## Software requirements

- Wolfram Mathematica 14.2
- Qiskit SDK 2.3.0
- Qiskit Runtime 0.45.0

## Reproduction

Each Mathematica notebook contains the payoff parameters used in the
corresponding figure. Evaluate the notebook from the beginning to reproduce
the numerical results and graphics.

## License

Code is released under the MIT License. Data are released under CC BY 4.0.
