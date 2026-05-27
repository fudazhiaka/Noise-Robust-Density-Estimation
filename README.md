Official implementation of Noise-Robust Density Estimation for Tabular Data Anomaly Detection (ICML2026)

How to use it:

```python
from NRDE import NRDE_run, read_data

file_path = "datasets/35_SpamBase.npz"
train_data, train_labels, test_data, test_labels, _, _ = read_data(file_path)
auroc, auprc = NRDE_run(train_data, train_labels, test_data, test_labels)
print(f"AUROC: {auroc:.3f}, AUPRC: {auprc:.3f}")
```
