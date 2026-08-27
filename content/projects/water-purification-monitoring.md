---
title: "Smart Water Treatment: Biodegradable Bio-Coagulant Hydrogel Beads"
date: 2026-05-15
status: Completed
tags:
  - Biotechnology
  - ESP32
  - Hardware
categories:
  - Projects
description: Combining Moringa oleifera seed hydrogel beads with an ESP32 microcontroller and turbidity sensor for real-time clarity monitoring.
---

     DATE OF COMPLETION: 20/05/2026

📌 Project Overview 
* **Goal:** Replacing synthetic, expensive chemical water treatments with eco-friendly hydrogel beads made from natural biomaterials and agricultural waste.
* **Smart Tech:** Integrated with an ESP32 microcontroller and turbidity sensor for automated visual feedback via LED indicators.
* **SDGs Targeted:** SDG 6 (Clean Water and Sanitation), SDG 12 (Responsible Consumption & Production), SDG 13 (Climate Action).

🧪 Science & Materials Behind the Beads 
1. Natural Biomaterials 
* **Moringa Seed Powder (*Moringa oleifera*):** Contains positively charged cationic proteins that neutralize negatively charged soil particles, causing them to form heavy flocs and drop to the bottom.
* **Banana & Orange Peel Powders:** Natural pectin, cellulose, and carboxyl functional groups actively bind contaminants via biosorption and surface ion interactions.
* **Activated Charcoal:** High-porosity carbon matrix designed for physical adsorption of suspended impurities.

2. Hydrogel Matrix Synthesis 
* **Sodium Alginate + Calcium Chloride ($\text{CaCl}_2$):** Sodium alginate acts as the encapsulating polymer matrix. Dropping the biomaterial-alginate mixture into a $\text{CaCl}_2$ solution triggers instant ionic crosslinking to form firm, biodegradable hydrogel beads.

🔬 Bead Formulation 
* **Step 1: Raw Materials Collection** – Collect moringa seeds, banana peels, orange peels, and charcoal.
* **Step 2: Slight De-Moisting** – Wash all materials and naturally de-moisten them to remove excess moisture.
* **Step 3: Grinding into Fine Powders** – Grind the dried materials separately into fine powders using a grinder.

|                     Moringa Powder                      |                   Banana Peel Powder                    |
| :-----------------------------------------------------: | :-----------------------------------------------------: |
|   <img src="/Images/moringa_powder.jpeg" width="300">   | <img src="/Images/banana_peel_powder.jpeg" width="300"> |
|                 **Orange Peel Powder**                  |                 **Activated Charcoal**                  |
| <img src="/Images/orange_peel_powder.jpeg" width="300"> |   <img src="/Images/charcoal_powder.png" width="300">   |

* **Step 4: Preparing Sodium Alginate Solution** – Dissolve sodium alginate in distilled water using a double-boiler setup to facilitate smooth dissolution without degrading the polymer.

<img src="/Images/double_boiler.jpeg" width="500">
*Figure 1: Double-boiler setup for dissolving sodium alginate.*

* **Step 5: Mixing All Powders into the Solution** – Add all prepared powders into the sodium alginate solution and mix thoroughly.
* **Step 6: Homogeneous Mixture** – Continue mixing until a smooth, uniform black slurry is obtained.
* **Step 7: Dripping into Calcium Chloride Solution** – Transfer the slurry into a syringe and drop it carefully into a $\text{CaCl}_2$ solution.

<img src="/Images/dripping_slurry.jpeg" width="500">
*Figure 2: Dripping biomaterial slurry into Calcium Chloride solution using a syringe.*

* **Step 8: Bead Formation (Cross-Linking)** – Allow calcium ions to cross-link with sodium alginate to form stable, spherical hydrogel beads. Leave them in the bath to solidify.

<img src="/Images/beads_in_solution.jpeg" width="500">
*Figure 3: Hydrogel beads curing inside the Calcium Chloride bath.*

* **Step 9: Washing** – Wash the formed beads multiple times with distilled water to remove remaining impurities.
* **Step 10: Drying** – Place the beads in a plastic petri dish and dry them completely.

<img src="/Images/drying_beads.jpeg" width="500">
*Figure 4: Synthesized hydrogel beads drying in a plastic petri dish.*

⚡ IoT Smart Sensor Setup & Qualitative Results 
Hardware Configuration 
* **ESP32 Microcontroller:** Processes sensor input to track water clarity in real time.
* **Analog Turbidity Sensor:** Works on a light-scattering mechanism to detect suspended particulate density.
* **Status LED Output:** Visual indicators wired directly to the ESP32.

Testing & Visual Outcome 
* **Procedure:** 250 mL soil-water samples were treated with equal bead doses, stirred gently for 1 minute, and left to settle for 10–15 minutes.
* **Observations:** Rapid floc formation, visible particle settling, and significant recovery of water clarity.

|                   Initial Contaminated Water                   |             Treated & Clarified Water              |
| :------------------------------------------------------------: | :------------------------------------------------: |
| <img src="../../../Images/contaminated_water.png" width="300"> | <img src="/Images/treated_water.jpeg" width="300"> |
|              *Raw turbid sample before treatment*              |       *Clear sample after 30 mins treatment*       |

* **Qualitative Indicator:** Once suspended particles settled and water clarity was restored, the ESP32 triggered the status LED to switch from red to green, signaling successful purification.

| Turbid Water (System Triggered) | Purified Water (Target Achieved) |
| :---: | :---: |
| <img src="/Images/circuit_red_led.jpeg" width="300"> | <img src="/Images/circuit_green_led.jpeg" width="300"> |
| *Red LED active during high turbidity* | *Green LED active post-purification* |
