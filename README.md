# 🐜 ACO with Dynamic Evaporation Rate – Adaptive Metaheuristic for Optimization

This project implements an enhanced **Ant Colony Optimization (ACO)** algorithm with a **dynamic pheromone evaporation rate** that adapts over iterations. This adjustment aims to balance **exploration** and **exploitation**, improving convergence on both **CEC benchmark functions** and **engineering optimization problems**.

---

## 🚀 Highlights

* 📉 **Dynamic Evaporation Rate:** The pheromone decay rate increases over time, shifting the search from exploration to exploitation.
* 📈 **Performance Evaluation:** Validated using **CEC Benchmark Suite** and real-world engineering test functions.
* 📊 **Statistical Testing:** Improvements confirmed via **Wilcoxon signed-rank tests** and visualized with convergence plots.
* 🧰 **Tools Used:** Python, NumPy, Google Colab, Matplotlib, Git

---

## ⚙️ Algorithm Overview

* Standard ACO uses a **fixed evaporation rate** (ρ).
* This version implements:

  ```
  ρ(t) = ρ₀ + (ρ_max - ρ₀) * (t / max_iter)
  ```

  Where:

  * ρ₀ is the initial evaporation rate
  * ρ\_max is the maximum allowed decay
  * `t` is the current iteration

This helps the colony explore broadly in the beginning and narrow down efficiently toward better solutions over time.

---

## 📊 Results Summary

* Achieved **faster and more stable convergence** on CEC functions (2014–2020).
* Outperformed baseline ACO in 9/12 benchmark problems (statistically significant at p < 0.05).
* Engineering test cases include:

  * Pressure vessel design
  * Gear train optimization

---

## 📚 References

* Dorigo, M., & Stützle, T. (2004). *Ant Colony Optimization*. MIT Press.
* Liang, J.J. et al. (2013–2020). *CEC Benchmark Functions*
* Wilcoxon Signed-Rank Test – Non-parametric statistical test for pairwise comparisons

---

## 🤝 Contributing

Contributions, feedback, and pull requests are welcome!

---


