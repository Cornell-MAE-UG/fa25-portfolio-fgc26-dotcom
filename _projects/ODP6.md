--- 
layout: project
title: "ODP 6: Client Report"
description: "Final Design and Report"
technologies: [python]
category: odp
image: /assets/images/ODP6CAD.png
--- 

## Context and Problem Statement

Spotted Lanternflies (SLFs), an invasive species rapidly spreading across the eastern United States, pose a growing threat to agricultural systems. SLFs land on grape vines and feed on plant sugars, contaminating harvests, reducing yields, and worsening grapes. SLFs also excrete honeydew, promoting growth of sooty mold that inhibits photosynthesis. These effects can cost the wine industry billions of dollars in lost yields.

On-vine SLF removal was shown to be impractical because the insects are numerous, and aggressive removal methods could damage the vines. Post-harvest removal proved to be too risky considering the high rate of contamination. Instead, our team explored whether there was a way to attract SLFs away from the vines completely.


---
## Final Prototype and Application

To lure SLFs away from grapevines, our system utilizes a sugary attractant designed to mimic the sap of the Tree of Heaven, a preferred host plant. Once lured to the device, SLFs are exterminated using targeted vinegar spraying through side-mounted sprayers.

**System Functions**

1. **Sap Attraction**  
   We pump a sugar solution that mimics the viscosity of natural sap through a central pole, creating an attractive feeding source.

2. **Targeted Elimination**  
   Once the insects gather, we spray them with vinegar using servo-actuated sprayers.

**Key Features**

- Adjustable spray angles for coverage optimization
- Compact footprint for vineyard integration
- Arduino-controlled automation
- Low-toxicity vinegar-based treatment

A vineyard simply places the device, turns it on, and it runs autonomously with minimal maintenance.

  <img src="{{ '/assets/images/ODP6 2.png' | relative_url }}" width="300">


---
**Assembly**

The system is designed so the box exterior can be rapidly assembled or disassembled if needed. Each panel contains a lip to maintain box geometry, while screws are attached throughout each panel for rigidity.

The lid of the box consists of two pieces that are loosely press-fit to the top of the box, giving quick access to the interior electronics and fluid reservoirs for maintenance. One panel contains a mounting profile for the electrical board, which is secured using four screws on the interior of the box.

Electrical components are wired together using jumper wires and Wago connectors that plug directly into the Arduino and allow for easy component connections in parallel.

A three-dimensional printed linkage allows servo motors to actuate the sprayer heads. A three-dimensional printed bar is screwed into the servo horn, pulling the actuator forwards and backwards. Everything is rigidly attached together using screws and mounted onto the top box panel.
<div style="display: flex; gap: 10px; justify-content: center; flex-wrap: wrap;">

  <img src="{{ '/assets/images/ODP6 3.png' | relative_url }}" width="30%">

  <img src="{{ '/assets/images/ODP6 4.png' | relative_url }}" width="30%">

  <img src="{{ '/assets/images/ODP6 5.png' | relative_url }}" width="50%">


</div>
---

## Testing Details and Results 

**Sap Drainage Test**

To test the longevity of the sap reservoir, we conducted a drainage test to determine how long the system could realistically operate in the field without being refilled.

**Procedure**

- Mixed 200 grams of sucrose with 300 grams of water to mimic Tree of Heaven sap viscosity
- Pumped solution for 10 minutes while recording water level every 2.5 minutes

**Results**

- Drainage rate: **0.5 milliliters per minute**
- Approximately **6 milliliters per day**
- A 1000 milliliter reservoir would require refilling approximately every **167 days**

<img src="{{ '/assets/images/Graph1.png' | relative_url }}" width="300">

---

## Spray Angle and Coverage Test

To confirm that the sprayers could cover the majority of the central pole in vinegar, we tested different sprayer angles to determine maximum coverage.

**Procedure**

- Covered the central pole in paper
- Set sprayers to a specific angle
- Performed a spraying cycle
- Measured the area of paper that became damp

**Results**

- Optimal working angle: **65 degrees**
- Spray coverage achieved: **86 percent**

This allowed coverage of most of the landing area for the Spotted Lanternflies on the system.

<img src="{{ '/assets/images/Graph2.png' | relative_url }}" width="300">

---

## Battery Life

To evaluate VineGuard’s power constraints, we calculated the system’s energy consumption.

**Results**

- VineGuard can operate for approximately **8.2 days** on a 10,000 milliamp-hour battery charge

The modular battery design enables users to balance cost against serviceability depending on deployment needs.

<img src="{{ '/assets/images/Graph3.png' | relative_url }}" width="300">

---

## Conclusion and Recommendation 

Based on our test results, VineGuard demonstrates strong potential as a feasible and effective solution for protection against Spotted Lanternflies. Our testing showed that the system can deliver the attractant at controlled flow rates, achieve ideal spray coverage under specific angles, and operate autonomously for extended periods with minimal maintenance once assembled.

Given this performance, we recommend continuing development of the prototype through vineyard field testing. Future testing should focus on evaluating attractant effectiveness, determining ideal placement locations, and improving aesthetics so the system better blends into vineyard environments.

Overall, VineGuard offers a feasible low-toxicity and low-intervention solution for mitigating Spotted Lanternfly damage in vineyards through a bio-inspired decoy system.

---
## Bill Of Materials

<img src="{{ '/assets/images/BOM2.png' | relative_url }}" width="700">

---

## References

[1] Amdro, “How to control and kill spotted lanternflies.”  

[2] CNBC, “Spotted lanternflies are feasting on United States grapevines and putting vineyards at risk,” October 13, 2022.  

[3] Cornell Chronicle, “Spotted lanternflies could cost New York State grape industry millions,” January 27, 2025.  

[4] BioNumbers (BNID 108683), “Viscosity of the sap (typically approximately five times water),” Harvard Medical School.  

[5] Penn State Extension, “Spotted lanternflies and beekeeping,” October 5, 2025.