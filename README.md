# GPU Mining Efficiency Analysis

This project analyzes GPU performance, energy efficiency, and algorithm support within the context of cryptocurrency mining.

Dataset used:  
[GPU Performance and Hashrate Dataset (Crypto) - Anthony Therrien](https://www.kaggle.com/datasets/anthonytherrien/gpu-performance-and-hashrate-dataset-crypto)

---

## 🎯 Project Objective

To evaluate mining performance of various GPUs by measuring:
- The number of supported mining algorithms per GPU
- Power consumption across algorithms
- Efficiency metrics (hashrate per watt)
- Top-performing GPUs in terms of energy and speed

---

## 📁 Directory Structure

```text
GPU_energy/
├── data/                          # Raw CSV files
├── images/                        # Exported plots
│   ├── energy_efficiency_best_gpus.png
│   ├── gpu_algo_supported_count.png
│   ├── gpu_energy_consumption_boxplot.png
│   └── top5_efficient_gpus.png
├── notebook/
│   └── gpu_energy.ipynb           # Main analysis notebook
├── requirements.txt              # Python dependencies
└── README.md
```

All plots are created via exploratory data analysis (EDA) using Jupyter.

---

## 📊 Dataset Summary

- 160+ unique GPU models
- 110+ columns with:
  - Hashrate metrics for 40+ algorithms
  - Power consumption in Watts
  - GPU manufacturer and model metadata
  - Energy cost estimates (per algorithm)

---

## ⚙️ Methodology

- **Cleaning**:
  - Dropped columns with excessive missing values
  - Clipped outliers for power usage
- **Feature Metrics**:
  - `algo_count`: Supported algorithm count per GPU
  - `algo_efficiency`: Sum of hashrates / total power consumption
- **EDA**:
  - Visual analysis of efficiency distribution
  - Algorithm support heatmaps
  - Boxplots of energy usage extremes

---

## 🔍 Key Findings

- 🔹 **Most Efficient GPU**: `6400` (AMD)
- 🔹 **Top Algorithm Support**: `3080Ti`, `3090` (NVIDIA)
- 🔹 **Power-Hungry Algorithms**: `Ethash`, `Octopus`, `Autolykos2`
- 🔹 **Efficiency Trend**: Some older GPUs offer better efficiency per watt despite lower absolute performance

---

## 🖼️ Visual Outputs (Found in `/images/`)

- `gpu_algo_supported_count.png` → Algorithms per GPU
- `energy_efficiency_best_gpus.png` → Overall energy efficiency
- `top5_efficient_gpus.png` → Top 5 energy-efficient GPUs
- `gpu_energy_consumption_boxplot.png` → Power usage outliers

---

## 🧰 Tools Used

- **Python 3.9**
- **Pandas**, **NumPy** – Data handling
- **Matplotlib**, **Seaborn** – Visualization
- **Jupyter Notebook**

---

## 📌 Future Improvements

- ROI-based ranking (cost vs. efficiency vs. hash power)
- Add market price to evaluate payback period
- Model performance across algorithm-specific benchmarks
- Time-based analysis if temporal data becomes available

---

## 👤 Author

**Hakan Ataş**  
Data Scientist | Blockchain Developer | Crypto Analyst | Trader

Project developed as part of a technical portfolio to evaluate mining hardware based on energy efficiency, performance, and algorithmic breadth.
