---
layout: page
title: Face Mask and Body Temperature Monitoring System
description: An embedded health and safety screening system using a Raspberry Pi, CNN-based face mask detection, and non-contact temperature sensing.
img: assets/img/face_mask_monitoring_diagram.png
importance: 2
category: research
---

{% include figure.liquid path="assets/img/face_mask_monitoring_diagram.png" title="Face mask and temperature monitoring system" class="img-fluid rounded z-depth-1" %}

This project presents an embedded face mask and body temperature monitoring system developed using a Raspberry Pi 4 and convolutional neural network (CNN) techniques. The system integrates distance sensing, computer vision, deep learning, and non-contact temperature measurement to provide automated health and safety screening.

An ultrasonic sensor first measures the distance between the system and the person. When the detected distance is within the predefined range of 10–60 cm, the system captures an image and detects the person's face. The detected face region is then processed by a trained CNN model, which classifies whether the person is wearing a face mask or not.

In parallel, a non-contact infrared temperature sensor measures the person's forehead temperature. The Raspberry Pi combines the mask-classification and temperature measurements through a decision-making process. If the person is wearing a mask and has a body temperature below 38.5°C, the system allows access without triggering an alarm. Otherwise, the system activates an alarm, indicating either the absence of a face mask or an elevated temperature.

The project demonstrates how embedded systems, computer vision, and deep learning can be integrated to develop a low-cost, automated solution for real-time health and safety monitoring.
