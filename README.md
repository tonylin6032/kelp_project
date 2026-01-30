# Kelp Early-Warning Signals Project

Goal: build kelp canopy time series from Landsat-derived pixels, define collapse events, compute early-warning signals, and relate to SST.

## Setup
Create a venv (example):
- python 3.10 recommended
- install: numpy pandas xarray netCDF4 matplotlib scipy ipykernel

## Data
Large data files are not tracked in git.
Place data under `data/`:
- Landsat kelp NetCDF: `data/LandsatKelpBiomass_2025_Q3_v2_withmetadata.nc`
- SST quarterly CSV (generated): `data/sst_quarterly_bbox.csv`

## Notebooks
- Use your main notebook to:
  1) extract bbox kelp series (saved CSV)
  2) load/clean
  3) merge with SST
  4) collapse + EWS
