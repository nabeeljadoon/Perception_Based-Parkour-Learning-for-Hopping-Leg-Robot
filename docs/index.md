---
title: "Summer of Underactuation 2024"
author: Dennis Mronga, Shubham Vyas
github: https://github.com/dfki-ric-underactuated-lab/
---

![Summer of Underactuation 2024 Group Photo (left to right: )](static/figures/summer_of_underactuation_2024.png)

# Event Summary

The  [Underactuated Lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/underactuated-lab/) at [DFKI Robotics Innovation Center](https://robotik.dfki-bremen.de/en/startpage.html) is committed to pushing the limits of our robots to achieve animal-like physical/athletic intelligence. Our lab generally hosts a bunch of exchange students with diverse backgrounds from all over Europe with a shared vision of developing athletic intelligence for underactuated robotic systems. The Summer of Underactuation 2024 event intends to highlight the scientific work of the exchange students working with the underactuated lab to everyone working at DFKI-RIC. We would like to invite you to join us on 31st July 2024 (Wednesday) from 14:00 to 17:00 in the B0.10 seminar room to enjoy (among others) quadruped locomotion in uneven terrain, real-time obstacle detection for a parkour hopping robot, monkey-like brachiation movements, humanoid state estimation, and optimal pendulum swing-up. Free pizzas will be provided for all the attendees afterwards.

| Time Slot      | Presentation                                                                                    | Speakers             |
|----------------|-------------------------------------------------------------------------------------------------|----------------------|
| 14:00 - 14:05  | Welcome Note                                                                                    | Prof. Frank Kirchner |
| 14:05 - 14:15  | Underactuated Lab Introduction                                                                  | Dr. Dennis Mronga, Shubham Vyas |
| 14:15 - 15:00  | Presentations                                                                                   | Hannah Isermann, Nabeel Jadoon, Jakob Middelberg  |
| 15:00 - 15:15  | Coffee break                                                                                    |         |
| 15:15 - 16:00  | Presentations                                                                                   | Lasse Hohmeyer, Mani Krishna, Adriano del Rio Fernandez |
| 16:00 - 16:30  | Demo session               |     |
| 16:30 - 17:00  | Late Lunch                 |     |

![The underactuated lab hosted students from all over the world in the past!](static/figures/student_map.png)

# Event Video Proceedings

In the following, you can find the proceedings from the event with the talks and abstracts.

## Forword by Prof. Frank Kirchner

Prof. Frank Kirchner gives a forword and explains the idea of the Underactuated Lab. 

<video src="static/videos/Frank2.mp4" controls="controls" style="max-width: 48em;"> </video>

## Underactuated Lab Past and Present

This talk by Dr. Dennis Mronga (Team leader Mechanics & Control at DFKI RIC) introduces the Underactuated Robotics Lab's past achievements and the current works. 

<video src="static/videos/Dennis2.mp4" controls="controls" style="max-width: 48em;"> </video>

## Underactuated Lab Next Steps

Shubham Vyas (Leader Underactuated Lab) presents the roadmap and vision for the lab for the next year.

<video src="static/videos/Shubham2.mp4" controls="controls" style="max-width: 48em;"> </video>

## Adaptive Gait Planning for Model Predictive Control of a Quadruped Robot by Hannah Isermann

While most current legged robots use fixed gaits for their locomotion, animals usually adapt their gait with increasing velocity. This behavior reduces the required energy and can increase stability while walking. In the work presented here, a biomimetic approach was followed to implement a gait sequencer which can autonomously adapt the gait parameters of a quadruped robot. Experiments on a field trip to Vulcano island were conducted to evaluate the new approach. The results show that the proposed gait sequencer reduces the required cost of transport, while simultaneously increasing the stability of the robot in rough terrain. 

<video src="static/videos/Hannah2.mp4" controls="controls" style="max-width: 48em;"> </video>

## Perception Based Parkour Learning for Hopping Leg Robot by Nabeel Jadoon

The research presented here investigates the integration of real-time perception into parkour navigation for underactuated legged robots. The currently implemented approach uses a mixed-integer programming (MIP) algorithm, which efficiently plans feasible paths through (known) obstacles, while a PD controller with feedforward torques executes the planned motions in real-time. Inspired by the human ability to navigate complex environments, we include real-time object detection through point cloud perception into the algorithm, which enhances the system's robustness and general applicability. The proposed approach is validated on a "Hopping Leg on a Boomstick" robot, demonstrating successful navigation of diverse and challenging parkour environments. This work highlights the potential of vision-guided control for achieving efficient and reliable locomotion in complex terrain for legged robots. 

<video src="static/videos/Nabeel2.mp4" controls="controls" style="max-width: 48em;"> </video>

## ARM vs x86: Performance comparison of different QP-Solvers by Jakob Middelberg

Modern robot control architectures for highly dynamic systems, such as bipeds or quadrupeds, often involve Model Predictive Control (MPC). This approach requires a mathematical optimization problem to be solved in real time. More specifically, a Quadratic Program (QP) is solved in the control loop by numerical algorithms, the so-called QP-Solvers. Since this control strategy involves a lot of computational resources, examining the efficiency of QP-Solvers could be helpful in finding an optimal solution for an onboard computer for a robotic system such as a quadruped. Hence, this research focuses on the comparison of different QP-Solvers on different hardware (computer) architectures. The performance of each solver is being assessed by calculating a “solve frequency per watt” metric. This allows for an easy comparison between solvers and architectures, respectively. 

<video src="static/videos/Jakob2.mp4" controls="controls" style="max-width: 48em;"> </video>

## Hybrid State Estimation for a Humanoid Robot by Lasse Hohmeyer

State estimation refers to all algorithms calculating the internal state of a robot. Since the true state is always unknown, it must be estimated based on noisy and inaccurate measurements. At present, model-based state estimation algorithms are the state of art in legged robotics, while data-driven approaches combining traditional model-based and data-driven methods have not been comprehensively explored yet. Therefore, the aim of the work presented here is the development, implementation and evaluation of a hybrid state estimation algorithm for the RH5 humanoid robot. A data-driven machine learning (ML) component will be integrated into the currently implemented model-based framework. Finally, some variants of the new hybrid algorithm should be evaluated against the current model-based algorithm for certain motions such as walking and single leg balancing. 

## Prototyping, Development, and Analysis of Different Contact Detection Methods for Bipeds and Quadrupeds by Mani Krishna Tippireddy

Bipedal and quadruped robots are advancing quickly, excelling in navigating difficult terrains and performing diverse tasks. Accurate foot-to-ground contact detection is crucial for their stability and balance, especially on uneven surfaces. The work presented here investigates various sensor-based methods for detecting foot-to-ground contact for these robots. It aims to evaluate their accuracy, robustness, and computational efficiency. The study involves a thorough literature review, selection of promising methods, and designing a compatible foot structure for testing. Experimental validation and comparative analysis are used to identify the most effective detection method. 

<video src="static/videos/Manikrishna2.mp4" controls="controls" style="max-width: 48em;"> </video>

## Data-driven modeling and optimal manipulator control by Adriano del Rio

In control, linear systems are generally desirable. In the case of model predictive control (MPC) the benefit of a linear system representation is significant, as it implies convexity of the optimization problem and global optimality for every solution. In this context, the Koopman operator theory is of high interest, as it evolves measurements of a system in a linear function space. Motivated by the enormous potential, the work presented here focuses on developing data driven Koopman models for predictive control of robotic manipulators with a serial architecture. Two Koopman based approaches were applied to single and double pendulum and compared to local linearization based MPC. 

<video src="static/videos/Adriano2.mp4" controls="controls" style="max-width: 48em;"> </video>



