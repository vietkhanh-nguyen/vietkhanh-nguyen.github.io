---
layout: single
title: "Multi-UAVs formation control project"
category: master_project
excerpt: "This is my Master 2 personal project"
date: 2025-12-01
slidesurl:
paperurl: "files/projects/consensus_quadcopter_project/report_final.pdf"
permalink: 
thumbnail: "/files/projects/consensus_quadcopter_project/Multi-UAVs.png"
---

Preface
======
This project was completed during the first semester of my Master 2 program in Smart Aerospace and Autonomous Systems, shortly after I arrived in France. I have been interested in formation control for a long time, but only recently had the opportunity to study it in depth. Therefore, this project was developed both as a way for me to practice consensus control and to gain a complete understanding of the control pip eline for drones. Most of the formation control knowledge I acquired comes from the book [1](https://sites.google.com/view/minhhoangtrinh/publications/dieu-khien-he-da-tac-tu), while the translation-scaling formation control approach is based on [2](https://arxiv.org/abs/1506.05636). All the control systems I designed were implemented in Python and simulated using MuJoCo. The project is public on my GitHub [here](https://github.com/vietkhanh-nguyen/multi-UAVs_formation_control).

My contribution
======
* Consensus algorithm is use for formation control. I use the bearing-based approach. Also I ensure the collision avoidance between agents.
* Developed an A* path-finding algorithm for static obstacle avoidance and path finding.
* A low-level thrust PID control for quadcopter.
* Documented the system architecture and algorithms, providing clear guidelines for the project.

![Multi-UAVs formation control in Mujoco](/files/projects/consensus_quadcopter_project/Multi-UAVs.png)

Simualation result
======
<div style="text-align: center; margin-bottom: 1em;">
  <video width="512" height="512" controls style="display: inline-block;">
    <source src="/files/projects/consensus_quadcopter_project/mj_consensus_video.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <br>
  <figcaption style="margin-top: 0.5em; font-style: italic;">Consensus control simulation</figcaption>
</div>

<div style="text-align: center; margin-bottom: 1em;">
  <video width="512" height="512" controls style="display: inline-block;">
    <source src="/files/projects/consensus_quadcopter_project/mj_tracking_video.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <br>
  <figcaption style="margin-top: 0.5em; font-style: italic;">Tracking control simulation</figcaption>
</div>



