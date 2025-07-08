# GPU Performance and Crypto Mining Analysis

This project analyzes GPU performance, energy efficiency, and algorithm support within the context of cryptocurrency mining.

Dataset used: [GPU Performance and Hashrate Dataset (Crypto) - by Anthony Therrien](https://www.kaggle.com/datasets/anthonytherrien/gpu-performance-and-hashrate-dataset-crypto)

---

## Project Objective

The goal is to explore the mining efficiency of various GPU models by evaluating:
- The number of algorithms supported per GPU
- Energy consumption across mining algorithms
- Energy-based efficiency metrics
- Identification of top-performing GPUs

---

## Directory Structure

GPU_energy/
├── data/
│ └── (Raw CSV files)
├── images/
│ ├── energy_efficiency_best_gpus.png
│ ├── gpu_algo_supported_count.png
│ ├── gpu_energy_consumption_boxplot.png
│ ├── top5_efficient_gpus.png
├── notebook/
│ └── gpu_energy.ipynb
├── README.md
└── requirements.txt


All images were generated through exploratory data analysis.  
Notebook includes feature calculations, cleaning, and visual output generation.

---

## Dataset Summary

- Total GPUs: 160+
- Columns: 110+
  - Hashrate metrics for 40+ mining algorithms
  - Power consumption per algorithm (Watt)
  - GPU model categories
  - Energy cost estimates

---

## Methodology

- **Cleaning**: Removed columns with excess NaNs, handled outliers.
- **Feature Engineering**: Only based on **existing** columns, no artificial features were added.
- **Key Metrics**:
  - `algo_count`: Number of supported algorithms per GPU
  - `algo_efficiency`: Total hash performance divided by total power
- **EDA**: Visualized top GPUs by efficiency, algorithm support, and energy distribution

---

## Highlights

- **Most Efficient GPU**: `6400` — belongs to AMD
- **Most Algorithm Support**: `3080Ti` and `3090` lead
- **Most Power-Hungry Algorithms**: `Ethash`, `Autolykos2`, `Octopus`
- **Boxplot Insight**: Several algorithms have extreme outliers in power usage

---

## Visual Outputs (Located in `/images`)

- `gpu_algo_supported_count.png`: Algorithm support count per GPU
- `energy_efficiency_best_gpus.png`: Overall efficiency distribution
- `top5_efficient_gpus.png`: Top 5 most energy-efficient GPU models
- `gpu_energy_consumption_boxplot.png`: Power usage variation per algorithm

---

## Tools Used

- Python 3.9
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

---

## Future Work

- Add ROI-based analysis combining cost, efficiency, and algorithm difficulty
- GPU recommendation engine per algorithm
- Time-series modeling if temporal data becomes available

---

## Author

**Hakan Ataş** – Data Scientist & Crypto Analyst & Blockchain Developer & Trader & Tıpan's father(Dog)❤️🐶
Project built for technical portfolio and mining hardware evaluation purposes.