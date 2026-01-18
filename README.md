# Periodic Autoregressive (PAR(1)) modelling of quarterly inflows (Spain – gauging station 9087 Grisén)

This repository provides a reproducible workflow (Google Colab + Google Drive) to:
- load daily gauging data exported from the Spanish *Anuario de Aforos* (MITECO) as SpreadsheetML/XML,
- compute quarterly (hydrological-quarter) inflows in hm³,
- fit a periodic autoregressive model PAR(1),
- generate synthetic equiprobable series,
- compute Q75 using the Gringorten plotting position,
- perform basic normality checks on the transformed/standardized series,
- export key tables/figures to Excel/PNG.

## Quick start (Google Colab)
1. Open the notebook in Colab (badge will work once the repo is on GitHub):
   - `notebooks/PAR_project_Colab.ipynb`
2. Upload the XML exported from MITECO when prompted.
3. The notebook will save outputs to your Drive under `MyDrive/PAR_project/outputs/`.

## Data source
Data originate from the MITECO *Anuario de Aforos* (free access).
Source statement: “© Ministerio para la Transición Ecológica y el Reto Demográfico”.

## Repository layout
- `data/raw/`: original XML exports (optional to include here)
- `data/processed/`: derived datasets (CSV/Excel) (optional)
- `notebooks/`: Colab-ready notebook
- `outputs/`: example outputs (optional)
- `src/`: helper utilities (optional)

## License
See `LICENSE`.

## How to cite
See `CITATION.cff`.
