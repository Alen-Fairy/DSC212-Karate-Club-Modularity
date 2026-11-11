# DSC212 — Modularity on the Karate Club Graph

This repository contains the Jupyter notebook for the DSC212 Graph Theory research assignment.

## Files
- `Karate_Club_Modularity.ipynb` — complete runnable notebook.
- `visualizations/` — generated graph and metric plots (created when the notebook is run).

## Run
1. Open the notebook in Google Colab or Jupyter.
2. Run all cells from top to bottom.
3. The notebook uses the built-in NetworkX Karate Club dataset and requires no manual dataset download.

## Dependencies
- Python 3
- NetworkX
- NumPy
- Pandas
- Matplotlib
- IPython

If needed, install with:
```bash
pip install networkx numpy pandas matplotlib ipython
```

## Method note
The recursive method uses the principal submatrix of the original global modularity matrix for each community, following the assignment handout. Node metrics are calculated on each node's current community-induced subgraph so their evolution reflects the changing community structure.

## Reference
Newman, M. E. J. (2006). Modularity and community structure in networks. PNAS, 103(23), 8577–8582. https://doi.org/10.1073/pnas.0601602103
