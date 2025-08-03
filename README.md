# DS5110-25Summer-Project

## Creating a data visualization dashboard for monitoring key metrics and performance indicators in a manufacturing plant

This project presents an **interactive dashboard application** for exploring two real-world datasets:

- **Smart-Grid Dataset** — energy metrics like power consumption, renewable generation, overloads  
- **Industrial-Safety Dataset** — accident reports, risks, and textual descriptions

The goal is to provide **real-time, user-centric insights** for energy planning and workplace safety, using data pre-processing, visualization, and predictive modeling techniques.

---

### Features

- **Multi-tab Dashboard** built with Python Plotly Dash:
  - Smart-Grid overview with time-series filtering
  - Safety dashboard with categorical trends and word cloud of accident causes
  - Forecasting module using regression models on monthly accident trends

- **Word Cloud Visualization** to reveal key risk terms from accident descriptions

- **Machine Learning Forecasting**:
  - Linear Regression and Decision Tree Regressor
  - MSE and R² evaluation for monthly accident predictions

---

### How to Run

Clone this Repo:
```
git clone https://github.com/huqingyuan314/DS5110-25Summer-Project.git
```

Run `smart_grid.ipynb` and `industrial_safety.ipynb` code blocks in sequence, then open `http://127.0.0.1:8050` in your browser.

> **Note:** To switch between different dashboard versions running on port `8050`, you may need to terminate the currently running process. Use the following commands in your terminal:

```bash
# Identify the process using port 8050
lsof -i :8050

# Terminate the process by replacing <PID> with the actual process ID
kill <PID>
