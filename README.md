# Photoemission Simulation Data Repository

This repository contains raw simulation data and plotting scripts used to generate figures in the paper:

> **"Simulating photoemission performance of a nanostructured bialkali photocathode with a 3D coupled finite difference time domain – Monte Carlo technique"**  
> by M. Popov, S. Belousov, I. Valuev, A. Knizhnik, and B. Potapkin.

## Repository Structure

The repository is organized by figure:

- **`data_for_fig1/`** – Contains experimental data and simulation results for Figure 1
  - `EXP_DATA.txt` – Experimental quantum efficiency (QE) measurements
  - `QE_L_MPF=3nm.txt`, `QE_L_MPF=5nm.txt` – Simulated QE data with different mean free paths
  - `fig1_maker.ipynb` – Jupyter notebook to regenerate Figure 1

- **`data_for_fig4/`** – Parameter optimization data for Figure 4
  - `flat.d` – Absorption data for flat structure
  - `flux_oneD_*.d` – Absorption flux data for 1D grating parameter sweeps (width and height)
  - `fig_4_maker.ipynb` – Script to generate Figure 4

- **`data_for_fig6-7-9/`** – Polarization and emittance data for Figures 6, 7, and 9
  - `1D-p-polariztion.txt`, `1D-s-polariztion.txt` – QE for 1D grating under parallel and perpendicular polarization
  - `Flat.txt` – QE for flat reference structure
  - `twod_pi2.txt`, `twod_pi4.txt`, `twod_pi8.txt` – QE for 2D grating at different polarization angles
  - `Emittance_*.txt` – Emittance data for various structures
  - `fig_789_maker.ipynb` – Notebook to generate Figures 6, 7, and 9

- **`data_for_fig_11_and_8/`** – Absorption and field distribution data for Figures 8 and 11
  - `abs_flat.txt`, `oned_abs.txt`, `TwoD_abs.txt` – Absorption spectra
  - `*_p.txt` – Photon absorption fractions in different semiconductor regions
  - `8_11_fig_maker.ipynb` – Script to generate Figures 8 and 11

## How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/photoemission-data.git
   cd photoemission-data
   Navigate to the specific figure directory and run the corresponding Jupyter notebook to regenerate plots.

Data files are plain text (.txt or .d) and can be loaded with any data analysis tool.

Requirements
Python 3.8+, Jupyter Notebook, NumPy, Matplotlib, Pandas
