# Nitrate Anomaly Detection — Sliding Window

**Author:** Simone Mayers

- Fixed **W=1000**, **q=97.5**
- One-sided (upper-tail) rule: value ≥ percentile threshold
- First window: label all points; then only the new point each step
- Percentiles use NumPy's **linear** method

Run the notebook `overlapping-sliding-windows-anomaly-detection.ipynb` to:
- load the CSV
- run the sliding-window detector
- print TP/FP/FN/TN and the two accuracies
- save `nitrate_anomalies_plot.png` with anomalies highlighted
