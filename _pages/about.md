---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="about-container">
  <!-- Last Updated -->
  <p class="about-last-updated">
    <strong>Last updated:</strong> <span id="last-updated"></span>
  </p>
  <!-- Introduction Section -->
  <h2>Introduction</h2>
  <p>
    My name is <strong>Nguyen Viet Khanh</strong>, a senior student in the Automation and Control Program at the School of Electrical and Electronic Engineering, Hanoi University of Science and Technology (HUST). I have a strong academic background and hands-on research experience in motion control for mobile robots and intelligent control strategies. My long-term goal is to contribute to cutting-edge research in control systems and intelligent robotics, integrating machine learning and advanced control methodologies to develop robust and adaptive autonomous systems.
  </p>

  <!-- My Journey Section -->
  <h2>My Journey into Control Engineering</h2>
  <p>
    Growing up in Hanoi, Vietnam, I developed an early fascination with control engineering. My first encounter was at the 2010 Honda Conference, where I witnessed the ASIMO <strong>humanoid robot</strong>. Its ability to perform tasks and interact with humans seemed like something out of science fiction, igniting my passion for robotics and intelligent systems.
  </p>
  <p>
    In 2021, I began my undergraduate journey with the program <strong>Control Engineering and Automation</strong> at <strong>Hanoi University of Science and Technology</strong>. Transitioning to university during the COVID-19 pandemic was a challenging experience, but I adapted quickly. I joined the <strong>Mechatronic Engineering Group (MEG)</strong> laboratory to gain hands-on experience in research and control systems. This experience cemented my decision to dedicate myself fully to this field, a choice I consider one of the most fulfilling of my academic career. During this time, I explored advanced concepts and engaged in self-study, often staying up late, fueled by curiosity. This passion for learning resulted in several publications in prestigious journals and international conferences.
  </p>
  <p>
    Fortunately, I had a 4-month internship at National Taiwan Normal University. This internship made me realize that I desire to seek an advanced research environment abroad to expand my horizon. And just like a dream come true, after receiving the IDEX scholarship at <strong>Université Paris Saclay</strong>, I am pursuing <strong>Master 2 Smart Aerospace and Autonomous System</strong>.
  </p>

  <!-- Research Interests Section -->
  <h2>Research Interests</h2>
  <p>
    As I look toward my future in the field of Automatic Control at the Department of Electrical Engineering, I am particularly drawn to the intersection of <strong>Robust Control</strong>, <strong>Predictive Control</strong>, and <strong>Neural Networks</strong>. My undergraduate research experiences have instilled in me a strong passion for <strong>Model Predictive Control (MPC)</strong> and <strong>Sliding Mode Control</strong> techniques for autonomous systems, as they provide a powerful framework for addressing uncertainties and constraints in dynamic environments. Also I really want to learn about novel <strong>Trajectory planning</strong> for robot.
  </p>
  <p>
    My master’s program focuses on the mechanics and control of autonomous systems, such as <strong>unmanned aerial vehicle (UAV)</strong> and <strong>unmanned ground vehicle (UGV)</strong>. It provides a comprehensive foundation for understanding and designing intelligent machines by covering kinematic and dynamic modeling, system analysis, and advanced control methods.
  </p>
</div>

<style>
/* Reuse CV container styling */
.about-container {
  max-width: 900px;
  margin: 2rem auto;
  padding: 2rem;
  border-radius: 10px;
  line-height: 1.7;
  text-align: justify; /* uniformly distributed text */
}

/* Light theme */
body.light .about-container {
  background-color: #ffffff;
  color: #111111;
  border: 1px solid #d1d5db;
}

/* Dark theme */
body.dark .about-container {
  background-color: #0f1724;
  color: #e6eef8;
  border: 1px solid #1f2937;
}

/* Links */
.about-container a {
  color: inherit;
  text-decoration: underline;
}

/* Headings styling */
.about-container h2 {
  border-bottom: 3px solid currentColor;
  padding-bottom: 0.3rem;
  margin-top: 1.5rem;
  margin-bottom: 1rem;
  font-size: 1.5rem;
  text-align: left; /* headings left-aligned */
}

/* Last updated text */
.about-last-updated {
  margin-bottom: 1.5rem;
  font-style: italic;
}
</style>

<script>
const lastUpdatedElem = document.getElementById('last-updated');
if (lastUpdatedElem) {
  const lastModified = new Date(document.lastModified);
  const options = { year: 'numeric', month: 'long', day: 'numeric' };
  lastUpdatedElem.textContent = lastModified.toLocaleDateString(undefined, options);
}
</script>
