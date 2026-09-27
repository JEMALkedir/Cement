# Cement notebooks

This repository currently contains six exploratory Jupyter notebooks. The input data, package versions, and a validated end-to-end execution order are not included. The names below are orientation only; inspect each notebook's code and input cells before running it.

| Notebook | Orientation from filename |
| --- | --- |
| `Eku_FIXED_journal_quality.ipynb` | Eku analysis and journal figure/report draft |
| `ML_Trail_1.ipynb` | Machine-learning trial |
| `Untitled0.ipynb` | Unnamed exploratory notebook; purpose needs confirmation |
| `co2.ipynb` | CO₂ analysis |
| `strength01.ipynb` | Strength analysis variant |
| `strength1.ipynb` | Strength analysis variant |

## Reproducing an analysis

1. Clone the repository and create a Python 3 environment using `environment.yml`. The file deliberately specifies only the Python 3 kernel indicated by notebook metadata; it is **not** a complete dependency lockfile.
2. Open the notebook you intend to reproduce in Jupyter or Colab. Read its import and data-loading cells. Install any required packages in that environment and record their exact versions before reporting a reproducible run.
3. Obtain the original input data from its owner. Place a local copy under `data/raw/` and update notebook-local paths as needed. No dataset is supplied here, and no input filename, schema, license, or provenance is asserted.
4. Run one notebook from a clean kernel, top to bottom. Record the notebook name, Git commit, Python and package versions, input provenance and checksum, any random seeds and split settings, and execution date with the resulting files.
5. Write generated tables, figures, and models under `outputs/`. These paths are a convention for future work; existing notebooks have not been changed to use them. Do not interpret stored notebook outputs as independently reproduced results.

## Directory convention

- `data/raw/`: original inputs, kept unchanged locally.
- `data/processed/`: derived input tables, with transformation steps documented.
- `outputs/figures/`, `outputs/tables/`, `outputs/models/`: generated artifacts.

The directories include only `.gitkeep` placeholders. Their contents are ignored by Git by default. If data can be shared, document its provenance and permissions before adding it explicitly. This scaffold does not establish an execution order or claim that all six notebooks run in the same environment.
