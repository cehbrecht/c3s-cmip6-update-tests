# c3s-cmip6-update-tests

Synthetic CMIP6 NetCDF fixtures for checking xarray decoding and clisops processing.

- [Subsetting](notebooks/qc-subsetting.ipynb) checks combined time and geographic bounding-box requests.
- [Regridding](notebooks/qc-regridding.ipynb) checks bilinear remapping through xESMF and ESMPy.

```sh
conda env create -f environment.yml
conda activate c3s-cmip6-update-tests
jupyter lab notebooks
```

Open either notebook and run all cells in order. Each notebook builds its own fixtures and runs pytest through `ipytest`. To refresh an existing environment, run `conda env update -f environment.yml`.
