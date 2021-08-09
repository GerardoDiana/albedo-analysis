# Albedo Analysis
This repository contains samples scripts and common functions for reading and exporting Neo4j graphical data.

## Contents
TODO: replace hyperlinks
- [GSA_AlbedoProd_GOES_075_VIS02_2000_181.nc](https://www.google.com) : the data is stored in a NetCDF file and contains the albedo (the proportion of the incident light or radiation that is reflected by a surface) over the region of South America.
- [NetCDF_spatialGP.ipynb](https://github.com/GerardoDiana/albedo-analysis/blob/main/NetCDF_SpatialGP.ipynb) : This notebook contains the data preprocessing and model fitting and predicting of a Gaussian process using a Standard Variational Approximation method with inducing points.
TODO: (Diana) Add a repository containing the R codes for a implementation using sp_bayes, and add a descriptsion
- [r_implementation/](https://www.google.com) : directory containing R codes
- [Written Report](https://www.google.com) : write-up for the analysis using and Bayesian exact GP.


## Python virtual environment instructions
### The virtual environment used for NetCDF_spatialGP.ipynb
After cloning the repo, change directory one level up.
Execute the following to create/copy the virtual environment with necessary libraries.
Do not create a virtual environment within the AlbedoAnalysis repo.

```bash
# create virtual environment (outside the gds_framework directory)
$: python3 -m venv albedo_venv  # create virtual environment
$: cd albedo_venv
$: source albedo_venv/bin/activate
(albedo_venv): pip install -r requirements.txt
(albedo_venv): python -m ipykernel install --user --name myenv --display-name "Python (myenv)"
(albedo_venv): <whatever work you want to do>
(albedo_venv): deactivate
$: logout
```

