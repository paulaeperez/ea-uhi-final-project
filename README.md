# ea-uhi-final-project
This repo contains the final project for the Earth Analytics course at CU Boulder Earth Lab

This project is the start of a workflow to process ECOSTRESS LST data and downscale it from 70m resolution to a finer resolution, with the ultimate objective of aiding the City of Boulder and interested parties to understand Urban Heat Islands better.

## Data sources
This product version pulls data from the ECOSTRESS mission, specifically from the ECO2LSTE and ECO1BGEO products. Direct downloads or download links for testing and de-bugging can be [found here](https://e4ftl01.cr.usgs.gov/ECOSTRESS/).


## Setup (env install)
The repo has the following dependencies:

- pandas
- geopandas
- matplotlib.pyplot
- json
- h5py
- math
- requests
- os
- pathlib
- pyproj
- time
- zipfile
- Fernet
- numpy
- pyresample
- gdal
- earthaccess

The base conda environment can be configured by following [these steps](https://www.earthdatascience.org/workshops/setup-earth-analytics-python/setup-python-conda-earth-analytics-environment/).

Not included in the environment are the packages h5py, pyresample, earthaccess, and pyproj, which should be installed in addition to the `earth-analytics-python` environment. A complete YAML file [environment.yml](environment.yml) is included for your convenience to setup an environment `ea-uhi` for this project. Run the below command from this directory to create the necessary conda environment.

```bash
conda env create -f environment.yml
conda activate ea-uhi
```