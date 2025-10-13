---
layout: single
title: "Multi-objective Particle Swarm Optimization project"
category: bachelor_project
excerpt: "This is one of my project in the Taiwan internship."
date: 2025-05-20
slidesurl: '/files/projects/mopso_project_report.pptx'
# paperurl: "/files/bachelor_thesis.pdf"
# permalink: /projects/bachelor-thesis/
---

# Multi-Objective PSO (MOPSO) Algorithm Overview

This algorithm is a **hybrid Multi-Objective Particle Swarm Optimization (MOPSO)** with **simulated annealing–like temperature control** and a **mode switch** from single-objective to multi-objective optimization.

---

Main Workflow
======

1. **Main Loop**
   The algorithm iterates until the **temperature** (`temp`) drops below a minimum value:
   - Evaluate each particle using the **objective function(s)**.
   - **Before switching mode**:
     - Use a **single-objective function** (combinte path length, obstacle advoidance, etc.) to update `p_best` and `g_best`.
   - **After switching mode**:
     - Apply a **multi-objective evaluation** (e.g., path length, smoothness, obstacle avoidance).
     - Perform **fast non-dominated sorting** and **crowding distance** to select diverse Pareto-optimal solutions.
     - Combine results to update the new `p_best` and calculate global best base on the Patero front rank.

2. **Velocity and Position Update**
   - Update each particle’s velocity using:
     ```
     v = w*v + c1*r1*(p_best - x) + c2*r2*(g_best - x)
     ```
     or a weighted mean term in multi-objective mode.
   - Clamp positions within the map limits to avoid going outside boundaries.

3. **Temperature Reduction**
   - After each generation, reduce the temperature:  
     ```
     T <- alpha * T
     ```
     (acts like a cooling schedule to stabilize convergence).

4. **Result Extraction**
   - Perform final **non-dominated sorting** to obtain the **Pareto front** (best trade-off solutions).
   - Save the trajectories and visualize convergence (fitness curves, paths).
![Simulation result](/images/mopso_project/Figure_Map_Environment.png "Simulation result")
![Simulation result](/images/mopso_project/Figure_mopso_all_traj.png "Simulation result 2")

---

Key Features
======

- **Two-phase optimization**: single-objective → multi-objective.
- **Adaptive simulated-annealing acceptance** for worse solutions.
- **Fast Non-Dominated Sorting (NSGA-II style)** for Pareto selection.
- **Crowding distance** for solution diversity.
- Designed for **path planning** with obstacle avoidance in a 2D map.