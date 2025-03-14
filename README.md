## **Analysis of the FitzHugh-Nagumo Model**

### **Authors**
- Andrea F. Campos Pérez

---
### **Languages Used**

![Julia](https://img.shields.io/badge/Language-Julia-purple?style=for-the-badge&logo=julia)

---

### **Overview**
This repository contains a **Julia-based computational analysis** of the **FitzHugh-Nagumo (FHN) model**, a simplified representation of neuronal excitability. The model is used to study the dynamics of excitable systems, such as action potential generation in neurons and cardiac cells.

The repository includes:
- A Jupyter Notebook (`.ipynb`) with code for simulating the FHN model under different parameter conditions. **Please download for full visualization.**
- An HTML version of the notebook for easy viewing.
- Both files have explanations mainly in English with some comments in Spanish.

---

### **Background**
The **FitzHugh-Nagumo (FHN) model** is a two-variable simplification of the Hodgkin-Huxley model for neural excitability. It consists of a fast activator variable (membrane voltage) and a slow recovery variable (refractory process). The system is described by the equations:

**du/dt = u - (u³/3) - v + I**  
**dv/dt = ε (u + a - bv)**

where:
- **u** represents the membrane potential,
- **v** is a recovery variable,
- **I** is an external stimulus,
- **ε, a, b** are model parameters controlling excitability.

This model exhibits behaviors such as **stable equilibrium points, limit cycles, and excitability thresholds**, depending on the parameter settings.

---

### **Files in This Repository**

| File | Description |
|------|------------|
| `Model_FitzHugh_Nagumo_Analysis.ipynb` | Jupyter Notebook implementing and analyzing the FHN model |
| `Model_FitzHugh_Nagumo_Analysis.html` | HTML-exported version of the Jupyter Notebook for quick viewing |

---

### **Simulation Details**
The notebook explores:
- **Phase-plane analysis** of the FHN system.
- **Time-series simulations** for different values of external current \( I \).
- **Bifurcation analysis** illustrating how changes in parameters affect system dynamics.
- **Numerical integration techniques** used to solve the differential equations.

---

### **How to Run the Notebook**
1. Install **Julia** (version 1.6 or later).
2. Install Jupyter Notebook and required Julia packages:
   ```sh
   using Pkg
   Pkg.add(["DifferentialEquations", "Plots", "PyPlot", "IJulia"])
   ```
3. Clone this repository:
   ```sh
   git clone https://github.com/andreaf-campos/FitzHugh-Nagumo-Model.git
   cd FitzHugh-Nagumo-Model
   ```
4. Launch the Jupyter Notebook:
   ```sh
   jupyter notebook Model_FitzHugh_Nagumo_Analysis.ipynb
   ```
5. Run the notebook cells to visualize different simulations.

---

### **Future Directions**
- Extend the model to **spatially coupled FHN systems** for wave propagation analysis.
- Study the impact of **noise** on neuronal excitability.
- Implement **alternative numerical solvers** for better performance.

---

### **References**
- FitzHugh, R. (1961). *Impulses and physiological states in theoretical models of nerve membrane*. Biophysical Journal, 1(6), 445-466.
- Nagumo, J., Arimoto, S., & Yoshizawa, S. (1962). *An active pulse transmission line simulating nerve axon*. Proceedings of the IRE, 50(10), 2061-2070.
- Izhikevich, E. M. (2007). *Dynamical Systems in Neuroscience: The Geometry of Excitability and Bursting*. MIT Press.

---

### **License**
This project is licensed under the MIT License.

If you use this work in academic research, please cite the original authors and provide a link to this repository.
