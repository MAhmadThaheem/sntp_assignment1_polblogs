# SE4095 — Social Network Theory and Practice — Assignment #01
Political Blogs Network Analysis (Adamic & Glance, 2005)

## Project structure

```
.
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   └── polblogs.gml          # place the dataset file here (not committed by default)
├── outputs/
│   ├── figures/               # generated plots (.png)
│   └── tables/                # generated tables (.csv)
├── build_notebook.py          # script that generates/updates the master notebook
└── SNTP_Assignment01_Master.ipynb   # the master notebook (all parts, run top-to-bottom)
```

## Setup

### 1. Clone the repository
```bash
git clone <your-repo-url>
cd <your-repo-folder>
```

### 2. Create and activate a virtual environment

**macOS / Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

**Windows (PowerShell):**
```powershell
python -m venv venv
venv\Scripts\Activate.ps1
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Add the dataset
Download `polblogs.gml` from Mark Newman's network data page
(https://public.websites.umich.edu/~mejn/netdata/) and place it at:
```
data/polblogs.gml
```

## Running the notebook

Open and run top-to-bottom in Jupyter:
```bash
jupyter notebook SNTP_Assignment01_Master.ipynb
```

Or execute it headlessly from the command line (regenerates all outputs):
```bash
jupyter nbconvert --to notebook --execute --inplace SNTP_Assignment01_Master.ipynb
```

All random seeds are fixed (global seed = 42; Louvain community detection
is additionally run across seeds 0–4 as required for stochastic methods),
so results are reproducible on any machine.

## Regenerating the notebook from source

The notebook is built programmatically from `build_notebook.py` (this
keeps every part's markdown explanation and code cell version-controlled
as plain Python instead of raw notebook JSON, which makes diffs in Git
much cleaner). To rebuild after editing `build_notebook.py`:

```bash
python build_notebook.py
```

## Outputs

Running the notebook populates:
- `outputs/figures/` — degree distribution, network visualizations, community-colored plots
- `outputs/tables/` — data dictionary, preprocessing log, graph statistics, centrality rankings, evaluation metrics, etc.

## Notes

- Analysis is performed on the **Largest Weakly Connected Component**
  of the cleaned graph (see Part A for justification).
- Ground-truth political-orientation labels are used **only** in Part E
  (evaluation) — never during community detection or centrality
  selection, per the assignment's core rule.
