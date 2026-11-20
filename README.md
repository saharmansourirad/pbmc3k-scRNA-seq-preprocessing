# PBMC 3k scRNA-seq Preprocessing

A practical single-cell RNA-seq preprocessing workflow using **Scanpy** and the PBMC 3k dataset.

## Project Structure

```text id="t4m2x1"
pbmc3k-scRNA-seq-preprocessing/
├── README.md
└── 01_scRNA_seq_QC_and_Preprocessing.ipynb
```

## Notebook

**01_scRNA_seq_QC_and_Preprocessing.ipynb**

This notebook covers the initial processing steps required to prepare single-cell RNA-seq data for downstream analysis, including:

- Loading and exploring the PBMC 3k dataset
- Quality control (QC) metrics and visualization
- Filtering low-quality cells and genes
- Preserving raw gene expression counts
- Normalization and log transformation
- Highly variable gene selection
- Saving the preprocessed AnnData object

## Output Data

The notebook generates a preprocessed AnnData file:

`pbmc3k_preprocessed.h5ad`

This file is used as the input for downstream clustering and cell-type annotation.

## Downstream Analysis

The preprocessed dataset is used in the companion repository:

[PBMC 3k scRNA-seq Analysis](https://github.com/saharmansourirad/pbmc3k-scRNA-seq-analysis)

After running this notebook, download `pbmc3k_preprocessed.h5ad` and upload it when prompted by the downstream analysis notebook.

## Dataset

The workflow uses Scanpy's built-in PBMC 3k dataset (`scanpy.datasets.pbmc3k`). It contains peripheral blood mononuclear cells from a healthy donor and is commonly used for learning and demonstrating single-cell RNA-seq analysis.

## Main Tools

- Python
- Scanpy
- AnnData
- NumPy
- Pandas
- Matplotlib

## Notes

- This is an exploratory learning project demonstrating a standard single-cell RNA-seq preprocessing workflow.
- The output file is an intermediate dataset for downstream analysis and is not committed to this repository.
- The preprocessing workflow is designed to prepare the data for subsequent dimensionality reduction, clustering and cell-type annotation.
