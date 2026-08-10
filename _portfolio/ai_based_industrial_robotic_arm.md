---
title: "Vision-Integrated Robotic Arm & ARM-Based Motor Control"
excerpt: "Developed an automated robotic arm prototype integrating a custom-designed PCB, ARM M051 embedded C firmware, and a Raspberry Pi-based object classification model for vision-guided manipulation tasks."
collection: portfolio
header: { teaser:"500x300.png" }
---

<h2>Overview</h2>
In this project, I engineered a complete hardware-software system for a custom robotic arm prototype. The objective was to combine mechanical actuation with computer vision to perform intelligent, automated object manipulation and classification tasks.

<h2>Hardware Design & Embedded Control</h2>
To serve as the physical brain of the system, I designed a custom printed circuit board (PCB) to handle the power and control routing. To drive the mechanics, I developed specialized embedded C firmware for an ARM-based Nuvoton M051 microcontroller. This firmware utilized the I2C communication protocol to orchestrate precise, reliable motor control and coordinate the arm's multi-axis movements.

<h2>Computer Vision & Sensor Integration</h2>
To give the arm spatial awareness and autonomy, I integrated a Raspberry Pi equipped with a camera and a custom sensor suite. I deployed an object classification model directly onto this edge setup to process visual data in real time. This integration provided continuous environment sensing and closed-loop feedback control, allowing the hardware to dynamically adjust and execute automated manipulation tasks based on what the camera classified.
