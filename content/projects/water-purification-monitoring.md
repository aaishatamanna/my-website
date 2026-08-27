---
title: Comparative Study of Multifunctional Biodegradable Bio-Coagulant Beads for Smart Water Treatment Applications
description: A biodegradable, IoT-integrated system for purifying water using natural materials and real-time turbidity monitoring.
date: 2026-06-15
tags:
  - Biotech
  - Sustainable Materials
  - IoT
  - Embedded Systems
---

## Overview

This project presents biodegradable hydrogel bio-beads formulated from natural materials — Moringa seed powder, banana peel powder, orange peel powder, and activated charcoal — encapsulated within a sodium alginate matrix. These beads purify contaminated water through combined coagulation, adsorption, and biosorption mechanisms. A smart monitoring system, built using an ESP32 microcontroller and turbidity sensor, was integrated to evaluate purification performance through real-time turbidity tracking.

## The Problem

Conventional water treatment relies heavily on chemical coagulants such as alum and ferric salts. While effective, these chemicals generate harmful sludge, raise treatment costs, and introduce secondary environmental pollution. Natural coagulants like *Moringa oleifera* offer a sustainable alternative, but their effectiveness is typically assessed through inconsistent manual observation. There is a need for a standardized, biodegradable treatment method paired with objective, real-time performance measurement.

## Objectives

* Develop biodegradable hydrogel bio-beads using natural coagulant and adsorbent materials.
* Encapsulate these materials within a sodium alginate matrix for stability and controlled interaction with water.
* Integrate an ESP32-based turbidity monitoring system to quantify purification performance in NTU (Nephelometric Turbidity Unit).
* Comparatively evaluate different bead formulations for turbidity reduction efficiency.

## Working Principle

The system combines two purification mechanisms within a single bead:

* **Coagulation:** Moringa seed proteins carry a positive charge and neutralize negatively charged suspended particles, causing them to clump together and settle (floc formation).
* **Adsorption / Biosorption:** Banana peel powder, orange peel powder, and activated charcoal contain cellulose, lignin, pectin, and porous carbon structures that trap and bind contaminants.

These materials are held within a sodium alginate hydrogel, formed through ionic cross-linking with calcium chloride — a structure known as the **"egg-box model."** This matrix keeps the active materials stable and allowed controlled contact with the water being treated.

## System Design

### Treatment Module
Bio-beads are introduced into contaminated water, where their embedded materials interact with suspended particles through coagulation, adsorption, biosorption, and chelation — improving water clarity over time.

### Monitoring Module
A turbidity sensor connected to an ESP32 microcontroller continuously measures water clarity before and after treatment. Readings are processed and displayed via the serial monitor, with green and red LED indicators providing a simple visual signal of water quality.

## Bead Preparation Process

1. **Raw material collection** — Moringa seeds, banana peels, orange peels, and charcoal.
2. **De-moisting** — Materials washed and naturally dried.
3. **Grinding** — Dried materials ground into fine powders.

| Moringa Powder | Banana Peel Powder |
| :---: | :---: |
| <img src="../../../Images/moringa_powder.jpeg" width="300"> | <img src="../../../Images/banana_peel_powder.jpeg" width="300"> |
| **Orange Peel Powder** | **Activated Charcoal** |
| <img src="../../../Images/orange_peel_powder.jpeg" width="300"> | <img src="../../../Images/charcoal_powder.png" width="300"> |

4. **Alginate solution preparation** — Sodium alginate dissolved in distilled water (using a double-boiler setup).

<p align="center">
  <img src="../../../Images/double_boiler.png" width="300">
</p>
<p align="center"><em>Figure 1: Double-boiler setup for dissolving sodium alginate.</em></p>

5. **Mixing** — Powders combined into the alginate solution to form a homogeneous suspension.
6. **Bead formation** — Mixture dropped into calcium chloride solution, triggering ionic cross-linking via a syringe.

<p align="center">
  <img src="../../../Images/dripping_slurry.jpeg" width="300">
</p>
<p align="center"><em>Figure 2: Dripping biomaterial slurry into Calcium Chloride solution using a syringe.</em></p>

7. **Washing** — Beads rinsed with distilled water to remove impurities.
8. **Drying** — Beads dried until stable and ready for use.

<p align="center">
  <img src="../../../Images/drying_beads.jpeg" width="300">
</p>
<p align="center"><em>Figure 3: Final prepared hydrogel bio-beads.</em></p>

## Materials and Equipment

### Hardware
* ESP32 Development Board
* Optical Turbidity Sensor Module (Analog)
* 5V DC Adapter / Power Bank
* Solderless Breadboard and Jumper Wires
* Two 10 kΩ Resistors (voltage divider, 5V to 3.3V conversion)
* Red and Green LED Indicators with 220 Ω Resistors
* Sodium Alginate-Based Bio-Coagulant Beads
* Glass Beaker for Water Samples

### Software
* Arduino IDE with ESP32 Board Package
* C/C++
* Arduino IDE Serial Monitor

## Testing and Results

The system was evaluated across six test cases covering bead formation, treatment efficiency, sensor accuracy, and overall system integration:

* **Bead formation:** Beads formed as stable, spherical structures that maintained integrity without disintegration.
* **Treatment efficiency:** Contaminated water showed a clear, visible improvement in clarity after treatment.
* **Turbidity sensor:** Accurately detected and reported varying turbidity levels across different samples.
* **ESP32 monitoring:** Continuously processed and displayed sensor readings without interruption.
* **LED indication:** Correctly switched between green (safe turbidity) and red (high turbidity) based on threshold values.
* **Overall system:** All components operated together successfully, meeting the project's intended objectives.

|                   Initial Contaminated Water                   |                 Treated & Clarified Water                 |
| :------------------------------------------------------------: | :-------------------------------------------------------: |
| <img src="../../../Images/contaminated_water.png" width="300"> | <img src="../../../Images/treated_water.png" width="300"> |
|              *Raw turbid sample before treatment*              |          *Clear sample after 30 mins treatment*           |

|               Turbid Water (System Triggered)               |                Purified Water (Target Achieved)                |
| :---------------------------------------------------------: | :------------------------------------------------------------: |
| <img src="../../../Images/circuit_red_led.png" width="300"> | <img src="../../../Images/circuit_green_led.jpeg" width="300"> |
|           *Red LED active during high turbidity*            |              *Green LED active post-purification*              |

## Applications

* **Household water pre-treatment** — a simple first step to reduce turbidity before further purification.
* **Rural and remote water treatment** — low-cost, community-level purification without dependence on infrastructure.
* **Agricultural and irrigation use** — reduces suspended solids in water used for irrigation.
* **Educational and research use** — a hands-on tool for studying coagulation, adsorption, and biosorption.
* **Environmental monitoring** — real-time turbidity tracking for water bodies.
* **Emergency and disaster relief** — a lightweight, portable option for treating water during shortages.
* **Smart water quality systems** — combines sustainable purification with IoT-based monitoring.

### Portable Bio-Bead Kit Concept
The beads were also designed as a compact, ready-to-use kit — pre-packaged in zip-lock pouches for easy transport and distribution. Requiring no electricity or specialized equipment, the kit is suited for schools, NGOs, and community programs operating in areas with limited infrastructure, offering a low-cost pre-treatment option for water used in irrigation or non-potable applications.
<p align="center">
  <img src="../../../Images/biobead_kit.jpeg" width="300">
</p>
<p align="center"><em>Figure: Pre-packaged portable bio-bead kit (concept visualization, AI-generated).</em></p>

## Limitations and Future Scope

* Bead composition, porosity, and controlled-release characteristics can be further optimized for improved treatment performance.
* Additional sensors — pH, Total Dissolved Solids (TDS), dissolved oxygen, temperature, and conductivity — could be integrated for more comprehensive water quality analysis.
* IoT connectivity could enable remote monitoring and cloud-based data storage.
* Future work could extend the system to heavy metal removal, wastewater treatment, and community-scale purification.

## Relevance to Sustainable Development Goals

* **SDG 3 — Good Health and Well-Being:** Reduces exposure to contaminated water and supports healthier living conditions.
* **SDG 6 — Clean Water and Sanitation:** Provides an affordable, eco-friendly approach to improving water clarity.
* **SDG 9 — Industry, Innovation and Infrastructure:** Combines biotechnology with smart sensing for an innovative treatment approach.
* **SDG 12 — Responsible Consumption and Production:** Converts agricultural waste (banana and orange peels) into a value-added product.
* **SDG 13 — Climate Action:** Reduces dependence on synthetic chemicals in favor of biodegradable alternatives.

<p align="center"> <img src="../../../Images/sdg_collage.png" width="300"> </p> <p align="center"><em>Figure: Sustainable Development Goals alignment collage.</em></p>

## Conclusion

Building this system bridged biotechnology with practical IoT execution, demonstrating that sustainable agricultural waste can directly solve real-world clean water challenges through smart, local engineering.