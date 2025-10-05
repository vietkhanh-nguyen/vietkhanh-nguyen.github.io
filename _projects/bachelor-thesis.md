---
layout: single
title: "Bachelor Graduation Thesis"
category: books
excerpt: "This thesis is my main research at the Department of Automation, School of Electrical Electronics, Hanoi University of Science and Technology (HUST)."
date: 2025-06-18
slidesurl: '/files/bachelor_thesis_presentation.pdf'
paperurl: "/files/bachelor_thesis.pdf"
permalink: /projects/bachelor-thesis/
---

My contribution
======
To fill in the gap, this thesis builds upon my previous publication, consolidating and presenting the core contributions from those studies in a structured manner. 
* This study introduces, the flatness characterization of the approximate sloshing model. It then develops a flatness-based trajectory planning method aimed at improving system performance and reducing sloshing effects. Two
different strategies—rest-to-rest interpolation and time optimization—are proposed to generate these flat-based trajectories.
* The Extended State Observer (ESO) is used to estimate combined disturbances and model uncertainties. It also provides necessary state information for controlling the liquid system, which might not be directly accessible
through sensors.
* The Lyapunov-based Model Predictive Control (LMPC) approach, integrates concepts from both MPC and SMC. This method not only guarantees accurate trajectory tracking and control signal convergence
but also enables the handling of complex systems with multiple constraints, offering a more robust and efficient control strategy.
* The second proposed controller approach ehance the computational efficient while having the ability to constraint the sloshing height. Integrating TSMC with Control Barrier Functions (CBF) enhances robustness against model
uncertainties and disturbances while maintaining safety by constraining the maximum sloshing height. The barrier function is carefully analyzed to ensure these constraints are upheld, even in the presence of estimation errors.

The link to the practical experiment could be foud [here](https://www.youtube.com/watch?v=5opAmY9NtqE)

![Graphical abstract](/images/bachelor_thesis/graphical_abstract.jpg "Graphical abstract")
![Graphical abstract](/images/bachelor_thesis/graphical_abstract_2.jpg "Graphical abstract 2")
