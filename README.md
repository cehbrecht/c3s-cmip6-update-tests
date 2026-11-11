# c3s-cmip6-update-tests

Synthetic CMIP6 NetCDF fixtures for checking xarray decoding and clisops time and geographic bounding-box subsetting.

```sh
conda env create -f environment.yml
conda activate c3s-cmip6-update-tests
jupyter lab cmip6_subset_checks.ipynb
```

Run all cells in order. The final table shows the outcome of opening each fixture and running both subset requests. The notebook prints the package versions and any warnings or errors.
