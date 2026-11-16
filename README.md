# CEH_ILESLA
Repository for ILESLA and CEH Team Challenges project

## Environment Setup

This project uses Conda (`conda-forge`) to manage Python and geospatial dependencies (`xarray`, `netcdf4`, `cfgrib`, `cartopy`, `scikit-learn`).

### 1. Install Miniforge (if you don't have Conda)
Download and install [Miniforge](https://github.com/conda-forge/miniforge#install) for your operating system (Windows, macOS, or Linux).

### 2. Create and Activate the Environment
From the root of the repository, run:

```bash
conda env create -f environment.yml
conda activate era5-analysis
```

### 3. Register the Jupyter Kernel (Optional)
If you are using JupyterLab or VS Code notebooks, register the environment so it appears in the kernel picker:

```bash
python -m ipykernel install --user --name=era5-analysis --display-name "Python (era5-analysis)"
```

### 4. Updating the Environment
If new packages are added to `environment.yml` later in the project, update your local environment with:

```bash
conda env update -f environment.yml --prune
```
