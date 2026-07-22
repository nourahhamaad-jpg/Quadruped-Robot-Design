# 🤖 Quadruped Robotic Dog - Custom Mechanical Design

## 📌 Project Overview
This repository presents an original mechanical design for a quadruped robotic dog created using Autodesk Tinkercad. The project demonstrates core principles of robotics engineering, including structural chassis design, 3D component modeling, joint placement, and static balance calculations.

---

## 🏗️ 1. Mechanical Features & Structure

### Chassis & Head Assembly
* **Main Body (Chassis):** Rectangular frame designed to house inner electronics and motor drivers.
* **Head & Sensors:** Features an integrated head module with dual optical sensors (eyes) and protective ear mounts for structural realism.
* **Color Scheme:** Dark Metallic Gray / Slate finish for a modern industrial robot aesthetic.

### Leg Mechanics & Degrees of Freedom (DOF)
* **Hip Joints:** Cylindrical actuators connecting the legs to the chassis.
* **Leg Structure:** Symmetrical 4-leg support mechanism positioned at each corner to provide maximum static stability.
* **Total Degrees of Freedom:** 2 DOF per leg $\times$ 4 legs = **8 DOF Total**.

---

## ⚙️ 2. Motor Torque Calculation

To ensure the robot stands securely without joint slippage:
* **Estimated Mass ($m$):** $0.8 \text{ kg} \approx 7.84 \text{ N}$
* **Mass per Leg:** $0.2 \text{ kg} \approx 1.96 \text{ N}$
* **Arm Distance ($d$):** $0.08 \text{ m}$ ($8 \text{ cm}$)

$$\text{Torque } (\tau) = \text{Force } (F) \times \text{Distance } (d)$$
$$\tau = 1.96 \text{ N} \times 0.08 \text{ m} = \mathbf{0.1568 \text{ N}\cdot\text{m}}$$

> **Conclusion:** Standard Micro Servos (e.g., SG90 or MG996R) capable of producing $>1.5 \text{ kg}\cdot\text{cm}$ torque are sufficient for static equilibrium.

---

## ⚖️ 3. Center of Gravity (CoG) & Balance
* The Center of Gravity is centrally positioned beneath the primary chassis to maintain static equilibrium across the 4-leg support polygon.

---

## 🚶‍♂️ 4. Proposed Gait Pattern
* **Gait Type:** **Trot Gait** (Diagonal pair movement).
* **Description:** The robot moves dynamically by lifting diagonally opposite legs (e.g., Front-Right and Rear-Left) simultaneously while the other pair maintains ground contact to ensure static and dynamic stability during motion.

---

## ⚠️ 5. Expected Mechanical Challenges & Solutions
1. **Joint Slippage & Backlash:** 
   * *Solution:* Using high-precision servo brackets and secure joint locks.
2. **Foot Friction (Slippage on smooth surfaces):** 
   * *Solution:* Adding rubber/silicone pads at the base of each foot segment to increase traction.
3. **Overheating under Static Hold:** 
   * *Solution:* Optimizing leg angles in code to reduce holding torque when standing idle.---

## 🚶‍♂️ 4. Proposed Gait Pattern
* **Gait Type:** **Trot Gait** (Diagonal pair movement).
* **Description:** The robot moves dynamically by lifting diagonally opposite legs (e.g., Front-Right and Rear-Left) simultaneously while the other pair maintains ground contact to ensure static and dynamic stability during motion.

---

## ⚠️ 5. Expected Mechanical Challenges & Solutions
1. **Joint Slippage & Backlash:** 
   * *Solution:* Using high-precision servo brackets and secure joint locks.
2. **Foot Friction (Slippage on smooth surfaces):** 
   * *Solution:* Adding rubber/silicone pads at the base of each foot segment to increase traction.
3. **Overheating under Static Hold:** 
   * *Solution:* Optimizing leg angles in code to reduce holding torque when standing idle.
