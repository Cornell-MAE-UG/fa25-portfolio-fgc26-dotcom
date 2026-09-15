---
layout: project
title: Gyroscope Design
permalink: /projects/Gyroscope/
---

<img src="{{ '/assets/images/Gyroscope.png' | relative_url }}" width="500
">

As part of CUSail, I worked on the design of a gyroscope stabilization system intended to reduce roll and improve the stability of our autonomous sailboat. I developed the system in SolidWorks, beginning with calculations to determine the flywheel size and mass required to provide a stabilizing effect for our approximately 40 lb boat.

Based on these calculations, I designed a flywheel with a 12 cm diameter and 1.38 cm thickness, with a target mass of approximately 3 lb. The final flywheel was manufactured from brass, whose high density allowed us to concentrate a significant amount of mass within a relatively compact geometry. This increased the flywheel's rotational inertia while keeping the overall system small enough to integrate into the boat.

I also researched and selected an outrunner brushless motor compatible with a 6S power system to spin the flywheel at high speed. From there, I modeled the supporting components in SolidWorks, including the gimbal mount and structural supports, while considering clearances, mounting locations, and the forces produced by the rotating flywheel.
<img src="{{ '/assets/images/Motor.png' | relative_url }}" width="500
">

To evaluate the concept before integrating it into the full-size boat, I designed an arc-shaped testing support that mimicked the rolling motion of the sailboat. The prototype allowed the gyroscope assembly to move as the boat would when disturbed, providing a way to investigate how the spinning flywheel could resist changes in orientation and help stabilize the vessel.

Throughout the project, I moved from engineering calculations and component selection to CAD modeling, material selection, prototyping, and system integration. The project gave me experience applying concepts from rotational dynamics to a real mechanical system while designing around practical constraints such as weight, available space, manufacturability, and integration with an existing autonomous sailboat.