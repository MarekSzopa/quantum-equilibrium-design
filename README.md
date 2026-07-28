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
- `data/raw/` – raw IBM Quantum measurement counts.
- `data/processed/` – processed payoff estimates and statistical summaries.
- `source_data/Source_Data.xlsx` – numerical source data underlying
  the figures and supplementary tables.

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
