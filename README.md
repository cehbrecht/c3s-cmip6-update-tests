# c3s-cmip6-update-tests

Synthetic CMIP6 NetCDF fixtures for checking xarray decoding and clisops time and geographic bounding-box subsetting.

```sh
conda env create -f environment.yml
conda activate c3s-cmip6-update-tests
jupyter lab cmip6_subset_checks.ipynb
```

Run all cells in order. The final cell uses `ipytest` to collect and run the pytest tests defined in the notebook. Pytest reports the results for xarray decoding, time subsetting, bbox subsetting, and the expected bbox error on a projected grid without geographic coordinates.
