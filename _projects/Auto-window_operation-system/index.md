---
layout: post
title: Automatic Window Operation System
description:  
    Designed and built a dual-microcontroller (ESP32-S3/ESP23-C6) automated window system
    featuring an indoor and outdoor environmental sensing over ESP-NOW + Wi-Fi, a 3-mode state machine (AUTO/MANUAL/LOCK), and a closed-loop actuator control. Delivered as a fully working prototype with custom PCBs, a Wi-Fi dashboard, SD Card data logging, and safety interlocks (E-STOP, overcurrent protection, rain/wind response), taken from schematic design through firmware, enclosure fabrication, and bench validation.
skills: 
  - PCB Design (Altium Designer)
  - Breadboard prototyping
  - PCB Assembly
  - Soldering
  - ESP-NOW + Wi-Fi 
  - C/C++
  - PlatformIO
  - 3D Design (Fusion)

main-image: /whole_project1.png
---

---
## Project Highlights 
- Dual-microcontroller architecture: ESP32-S3 (indoor, high GPIO count for LCD, SD card, encoder, motor driver) paired with ESP32-C6 (outdoor sensing), communicating over ESP-NOW
- Closed-loop actuator control using a BTS7960 driver and potentiometer feedback for precise 0 to 100% window position
- Three-mode state machine (Auto, Manual, Locked) with a dedicated Teacher Override for session-based access control
- Layered safety priority chain: E-STOP, overcurrent/jam protection, natural event response (rain and wind), then mode dispatch
- Full data logging pipeline: SD card CSV storage at 5-second intervals, downloadable logs, and a live Wi-Fi web dashboard
- Custom PCB design in Altium with 3D-printed enclosures for both indoor and outdoor units
- Fully assembled, working prototype validated through bench testing (5 trials x 4 target positions), with 12-module firmware architecture built in C++/PlatformIO
 ---

## Indoor Module 
{% include image-gallery.html images="awo_in_pcb1.png,awo_in_pcb2.png,awo_in_pcb3.jpg,awo_in_pcb4.jpg,awo_in_assmbld1.jpg,awo_in_assmbld2.jpg" height="400" %} 
 


## Outdoor Module
{% include image-gallery.html images="awo_out_pcb1.png,awo_out_pcb2.png,awo_out_pcb3.jpg,awo_out_pcb4.jpg,awo_out_assmbld1.jpg" height="400" %} 

## Web Dashboard
{% include image-gallery.html images="dashboard1.png,dashboard2.png" height="400" %} 
