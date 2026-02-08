# A.D.A.M. v0.1 (Infrastructure-Independent Distributed Search Modules) 🤖

**A.D.A.M. v0.1** is a low-cost, mobile robotic sensor platform designed as a "forward eye" for search and rescue operations in disaster zones where critical infrastructure (GSM, GPS, Internet) has collapsed. This project serves as the first hardware iteration (v0.1) of the "Soldier" mobile units, aimed at establishing a robust Proof-of-Concept (PoC) for life detection in hazardous environments.

---

### ⚠️ Project Status

**Current Stage:** This project is currently in the **application approval stage** for the TÜBİTAK 2209-A Research Project Program. It is **not yet funded or officially supported** by any institution; all developmental progress is currently conceptual or at the preliminary prototyping stage.

---

### 🌟 Key Features (Sensor Fusion)

The platform integrates multiple sensing modalities into a single STM32-based embedded system to navigate and detect life under rubble:

* 
**Thermal Imaging:** MLX90640 sensor for detecting heat signatures/hotspots of survivors.


* 
**Acoustic Detection:** High-sensitivity microphone for locating cries for help or structural sounds.


* 
**Spatial Awareness:** Forward-facing ToF (Time-of-Flight) Laser for collision avoidance and distance measurement.


* 
**Stability:** MPU-6050 IMU to monitor the robot's orientation and balance in chaotic terrain.



---

### 🏗️ System Architecture

The v0.1 architecture focuses on a "Wired Command Center" model to ensure reliable data transmission in radio-silent zones:

* 
**Processor:** STM32 Development Board (programmed in Embedded C/C++).


* 
**Locomotion:** Tracked robot chassis for superior maneuverability over debris.


* 
**Connectivity:** Serial communication (USB-UART) via cable to a Command Center terminal.


* 
**Interface:** Real-time monitoring of sensor telemetry (Temperature, Distance, Audio Levels).



---

### 🎯 Success Criterion: The "Blind Operator" Test

The platform's success is measured by its ability to navigate a complex indoor obstacle course without direct line-of-sight. The operator must guide the unit solely through sensor feedback to identify heat and sound sources at the end of the course.

---

### 🗺️ Future Roadmap

* 
**v1.0 - v2.0:** Implementation of self-healing LoRa Mesh Networks for wireless operation.


* 
**v3.0:** Development of autonomous swarm intelligence algorithms.



---

### 🛡️ Ethical & Safety Standards

Development follows strict safety protocols for soldering and electronics handling, including proper ventilation and personal protective equipment (PPE). The project is designed with a "human-first" philosophy, aiming to reduce the risk to first responders.

---

### 🛠️ Hardware Stack

* 
**Main Micro:** ST Nucleo - F411RE 


* 
**Thermal:** MLX90640 


* 
**Distance:** VL53L0X ToF 


* 
**IMU:** MPU-6050 


* 
**Power:** 11.1V 3S LiPo
