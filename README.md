# Landmark Detection & Robot Tracking (SLAM)

This project implements **SLAM (Simultaneous Localization and Mapping)** for a **2D robot world**, as part of the **Udacity Sensor Fusion / Robotics curriculum**.  
The goal is to **track a robot’s position over time while simultaneously estimating the locations of landmarks**, using only noisy motion and sensor measurements.

---

## Project Overview

In this project, SLAM is implemented for a **two-dimensional grid world**.  
The robot moves through the environment while observing landmarks and estimating both:

- Its **own pose (x, y position)**
- The **positions of landmarks** in the environment

The system combines:
- Robot motion updates
- Noisy landmark measurements
- Constraint-based estimation (Omega–Xi formulation)

SLAM enables the robot to build a map of the environment **incrementally over time**, which is a fundamental capability in **autonomous robotics and navigation**.

---

## Example Output

Below is an example of a **2D robot world** with:
- **Purple “×”** → detected landmarks  
- **Red “o”** → robot final estimated position  

> This example corresponds to a **50×50 grid world**, but multiple map configurations can be generated.

![SLAM Example Output](robot_world.png)


---

## Project Structure

The project is organized into **three Python notebooks**, but **only the final notebook and robot implementation are graded**.

### Notebook Breakdown

- **Notebook 1 – Robot Moving and Sensing**  
  Introduces robot motion and noisy sensing models.

- **Notebook 2 – Omega and Xi Constraints**  
  Implements SLAM constraints using information matrices.

- **Notebook 3 – Landmark Detection and Tracking** 
  Full SLAM implementation combining motion and sensor constraints.

### Graded Files
- `robot_class.py`
- `Notebook 3 – Landmark Detection and Tracking.ipynb`

---

## Core Concepts Used

- Simultaneous Localization and Mapping (SLAM)
- Probabilistic robotics
- Constraint-based optimization (Omega–Xi)
- Noisy motion and measurement models
- Landmark-based mapping
- Graph-based state estimation

---

## How to Run

1. Open **Notebook 3** in Jupyter:
   ```bash
   jupyter notebook
