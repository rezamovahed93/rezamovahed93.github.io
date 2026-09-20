---
layout: page
title: Raspberry Pi-Based Vehicle Anti-Theft System
description: A facial-recognition-based vehicle access control system built on a Raspberry Pi, using face embeddings and cosine similarity matching.
img: assets/img/vehicle_antitheft_diagram.png
importance: 4
category: research
---

{% include figure.liquid path="assets/img/vehicle_antitheft_diagram.png" title="Raspberry Pi-based vehicle anti-theft system pipeline" class="img-fluid rounded z-depth-1" %}

This study presents a Raspberry Pi–based vehicle anti-theft system that uses facial recognition to authenticate individuals entering a vehicle. Upon entry, the system captures an image of the occupant, then detects and crops the face from the frame. A feature extraction model then encodes the cropped face image into a fixed-length feature vector (embedding). The cosine similarity between this vector and the stored embeddings of authorised users, whose facial data were previously enrolled in the system, is then computed. If the similarity score for any enrolled user exceeds 0.5, the system recognises the individual as that authorised user. Otherwise, the system classifies the individual as unauthorised, triggering the vehicle's alarm and sending an SMS notification to the owner.
