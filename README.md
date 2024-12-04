# Control of Wheeled Inverted Pendulum

This project models, simulates, and controls a **Wheeled Inverted Pendulum** system using MATLAB and Simulink. The project focuses on stabilizing the system's nonlinear and unstable dynamics using state-space control techniques like Linear Quadratic Regulator (LQR) and state feedback control. Additionally, a state observer is implemented to estimate unmeasured states for robustness.

---

## Table of Contents
- [Project Description](#project-description)
- [Features](#features)
- [Getting Started](#getting-started)
- [System Parameters](#system-parameters)
- [Simulation Results](#simulation-results)
- [How to Run](#how-to-run)
- [References](#references)

---

## Project Description

The **Wheeled Inverted Pendulum** is a benchmark problem in control theory, with applications in self-balancing robots and autonomous vehicles. This project addresses:
- Modeling using the Lagrangian approach.
- Linearization of the model for a state-space representation.
- Control design using State Feedback and LQR techniques.
- Observer design for state estimation and system robustness.

---

## Features

- **Dynamic Modeling**: System equations derived using Newton-Euler or Lagrangian methods.
- **Linearization**: State-space model linearized around the upright equilibrium.
- **Control Design**:
  - Pole Placement using Ackermann's Formula.
  - LQR for optimal control.
- **Observer Design**: Reconstructs unmeasured states.
- **Simulation**: Validates system behavior using MATLAB/Simulink.

---

## System Parameters

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <ul>
      <li><code>m_c</code>: Mass of the cart (kg)</li>
      <li><code>m_p</code>: Mass of the pendulum (kg)</li>
      <li><code>L</code>: Length of the pendulum (m)</li>
      <li><code>d1</code>, <code>d2</code>: Damping coefficients</li>
      <li><code>u</code>: Control force applied to the cart (N)</li>
      <li><code>q1</code>: Horizontal displacement of the cart (m)</li>
      <li><code>q2</code>: Angle of the pendulum from the vertical (rad)</li>
    </ul>
  </div>
  <div style="flex: 1; text-align: center;">
    <img src="Documents & Reports/Photos/Schemetic.png" alt="System Parameters Diagram" style="max-width: 100%; height: auto;">
    <p><i>Figure: Diagram representing system parameters</i></p>
  </div>
</div>

---

## Simulation Results

### Real-life Robot Photo
Here is a real-life implementation of a wheeled inverted pendulum robot for reference:

![Real-life Robot](Documents%20&%20Reports/Photos/Real%20Life.png)


### Simulink Simulation GIF
The following GIF demonstrates the system's simulation using MATLAB/Simulink:

![Simulation GIF](Documents%20&%20Reports/Photos/Output%20simulation.gif)

### Key Insights
1. **Open-loop System**: Unstable dynamics, as seen in the initial simulation.
2. **State Feedback Control**: Stabilized response using designed feedback.
3. **LQR Control**: Optimal trade-off between control effort and stability.
4. **Observer Implementation**: Accurate reconstruction of unmeasured states.

---

## Getting Started

### Prerequisites
- MATLAB (R2021a or later)
- Simulink
- Basic knowledge of state-space modeling and control theory.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/DavePreet/IE-415-Control-of-Autonomous-Project.git
