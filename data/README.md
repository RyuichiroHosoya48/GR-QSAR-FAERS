# Input data

Place the following input files in this directory before running the notebook.

## Files used in the reported analysis

- `20260407_BDB_GR_cSMILES_pKi dedup_descriptors_computed.csv`
  - GR binding-affinity training data used when `COMPUTE_DESCRIPTORS=True`
  - Required columns: `canonical_SMILES` and `pKi`

- `20260430_FAERS2025_druglist_cSMILES_real Pki.csv`
  - FAERS drug structures used for final prediction
  - Required column: `canonical_SMILES`
  - An optional `pKi` column may be included for the descriptive measured-versus-predicted comparison

## Optional precomputed-descriptor files

The notebook also contains paths for precomputed descriptors. These files are needed only when the corresponding precomputed-descriptor mode is selected:

- `20261017_2_BDB_GR_cSMILES_pKi dedup_descriptors_computed.csv`
- `20260430_FAERS2025_druglist_real pKi_predict_descriptors.csv`

The input datasets are not included in this repository. Binding-affinity data should be obtained from [BindingDB](https://www.bindingdb.org/), and FAERS source data should be obtained from the [FDA Adverse Event Reporting System](https://fis.fda.gov/extensions/FPD-QDE-FAERS/FPD-QDE-FAERS.html). Users are responsible for complying with the applicable terms of use and data-use conditions of the original data sources.

The input files should be prepared according to the procedures described in the accompanying manuscript. File names must match those listed above unless the corresponding paths in the notebook are modified.
