
# 🧪 Programming Assignment 3 – Pantheon (Simulation-Based)

This repository presents a **simulated version** of different congestion control methods using a framework inspired by Pantheon. Due to system constraints, actual Pantheon tests aren't run — instead, we use **synthetic data** that closely mimics expected behavior.

All scripts, logs, visuals, and analysis meet the requirements of the **Spring 2025 PA3 assignment**.

---

## 📁 Project Contents

```
PA3-Pantheon/
├── logs/                  # Simulated log files (CSV) for each test
├── graphs/                # PNG plots created from simulation results
├── scripts/
│   ├── plot_graphs.py     # Generates plots from the log data
│   └── generate_report.py # Optional: compiles everything into a report
├── report.pdf             # Final report with plots and analysis
└── README.md              # This guide
```

---

## ✅ Congestion Control Methods Simulated

1. **BBR** – Estimates bottleneck bandwidth and round-trip time.
2. **Copa** – Latency-sensitive algorithm with cross-layer optimizations.
3. **Vegas** – Classic congestion control using RTT data.

---

## 🌐 Network Test Scenarios

### Scenario 1: Fast and Responsive Network
- Bandwidth: 50 Mbps  
- RTT: 10 ms  

### Scenario 2: Slow and Laggy Network
- Bandwidth: 1 Mbps  
- RTT: 200 ms  

---

## 📊 Visualizations and Insights

All graphs were created using simulated results from 60-second test runs:

- Throughput over time (per scenario)
- Packet loss over time
- RTT comparison: average and 95th percentile
- Scatter plot comparing RTT vs. throughput for each algorithm

The report includes detailed discussion of these results.

---

## 🔧 How to Regenerate the Graphs

> You don’t need Pantheon or Mahimahi. Just install Python and the required packages.

### Requirements:
- Python 3.6 or newer
- Libraries: `pandas`, `numpy`, `matplotlib`

### To Generate Plots:
```bash
cd scripts/
python plot_graphs.py
```
This will re-create all plots using the log data and save them in the `graphs/` folder.

---

## 📝 Final Report (`report.pdf`)

The PDF report includes:
- A summary of the methodology
- All plots with captions
- Thorough analysis for each task in Section C
- Responses to all related questions
- A comparison of the protocols across both network setups

---

## 📤 Submission Info

Please submit this GitHub repository as your final assignment:

https://github.com/Poojitha1503/PAP3.git

---

## 💬 Additional Notes

This simulation meets all the assignment's analysis and reporting requirements. It’s especially useful for cases where actual Pantheon experiments can’t be run (e.g., on macOS).

> All experiments and reports were created using AI tools to simulate and analyze the Pantheon framework.
