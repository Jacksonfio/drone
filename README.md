# THREATVERSE — AI-Enabled 3D Drone & Counter-Drone Threat Simulation Trainer

[![System Status](https://img.shields.io/badge/System-ONLINE-15803d.svg)](https://github.com/Jacksonfio/drone)
[![Engine](https://img.shields.io/badge/3D%20Engine-Three.js%20WebGL-1d4ed8.svg)](https://threejs.org/)
[![License](https://img.shields.io/badge/License-Proprietary%20Defense%20Simulator-0f172a.svg)](LICENSE)
[![Physics](https://img.shields.io/badge/Physics-60%20FPS%20Kinematics-blue.svg)](https://github.com/Jacksonfio/drone)

**THREATVERSE** is a professional, military/defence-inspired simulation, analytics, and command-learning platform designed for training Counter-Unmanned Aerial Systems (C-UAS) observers, air defense operators, and security personnel.

The platform provides a realistic, human eye-level 3D simulation environment that models real-world physical terrain, atmospheric degradation, commercial and military UAV flight kinematics, and the cognitive stress of detecting, classifying, and responding to airborne threats under genuine operational uncertainty.

---

## 🌟 Key Platform Capabilities

### 1. Realistic Multi-Terrain 3D Environments
Instantly switch between four realistic operational environments:
* 🏙️ **Metropolis City Sector:** Dense commercial district with high-rise towers, multi-tier office complexes, illuminated window grids, rooftop HVAC equipment, communication antennas with hazard beacons, multi-lane asphalt highway grid, sidewalks, and streetlights.
* ⛰️ **Mountain Outpost & Valley:** Undulating mountain terrain with steep ridges, rocky peaks, elevated observation watchtower with searchlights, winding trails, and alpine pine forests.
* 🏡 **Rural Village & Farmland:** Village dwellings with pitched roofs and chimneys, agricultural barns, wooden perimeter fences, dirt paths, water towers, and scattered oak trees.
* ⚓ **Coastal Port & Industrial Asset:** Protected waterfront perimeter with water reflections, stacked shipping container terminals, industrial warehouses, and security fences.

### 2. High-Visibility Customizable Drone Hangar
Equipped with four customizable 3D UAV threat configurations:
* **Commercial Quadcopter (DJI Mavic / Phantom style):** 4 carbon-fiber arms, spinning rotors, landing skids, 3-axis gyro gimbal optical camera, and FAA/ICAO anti-collision strobe lights.
* **Fixed-Wing Reconnaissance UAV:** Aerodynamic surveillance glider with long wingspan, rear pusher propeller, and belly optical turret.
* **Industrial Heavy Hexacopter:** 6 radial motor arms, dual heavy-duty battery packs, and suspended threat cargo/payload module.
* **Micro-FPV Racing / Kamikaze Drone:** Ultra-compact high-speed racing quad with aggressive camera tilt and acrobatic evasion trajectories.

#### Real-Time Drone Customizer Controls:
* **Target Range & Distance:** Adjust engagement range from **Close Inspection (45m)** to **Tactical (140m)** and **Perimeter (350m)**.
* **Flight Altitude:** Adjust operating altitude from low-level rooftop skimming (12m) to high altitude (120m).
* **Flight Kinematics & Speed:** From stationary station-keeping hover to slow reconnaissance or high-speed evasive dash.
* **Threat Payload Selection:** EO/IR Surveillance Gimbal, Suspended Payload / Dropper, or Electronic RF Jammer Pod.
* **Navigation Lighting:** High-Visibility Strobes, Military Green/Red, Stealth (Lights Dark), or Warning Amber.
* **Flight Trajectories:** Stationary Hover, Figure-8 Recon Orbit, Direct Incursion Vector, or Building Slalom.

### 3. Dynamic Weather & Atmospheric Shaders
* ☀️ **Natural Daylight:** Directional sunlight with soft PCF cascaded shadows and high-contrast building silhouettes.
* 🌙 **Night Operations:** Low-light tactical night operations with subtle lunar illumination, glowing building windows, and localized streetlight cones.
* 🌫️ **Volumetric Dense Fog:** Exponential fog (`THREE.FogExp2`) reducing visibility to $<180\text{ m}$, creating authentic sensor noise and visual ambiguity.
* 🌧️ **Precipitation / Rain:** Volumetric 3,500-particle falling rain system with wet, specular asphalt ground reflections.

### 4. Interactive Observer Camera Suite
* **Observer Eye-Level:** Stand physically at the human observer post (+12m) overlooking the perimeter.
* **Target Track Lock:** Gimbal camera locks onto and dynamically tracks the selected drone across the 3D airspace.
* **Tactical Recon (Air):** Top-down satellite orthographic 3D grid (+320m) for complete battlespace situational awareness.
* **Free Orbit:** Full 360° mouse drag, tilt, pan, and scroll wheel inspection.
* **PTZ Optical Zoom:** 1.0x to 8.0x digital/optical zoom with live Field of View (FOV) adjustment.

### 5. Signature Feature: *"What Did I Know Then?"*
An After-Action Review (AAR) historical timeline scrubber that eliminates hindsight bias. When reviewing past sessions, instructors and trainees can scrub second-by-second to inspect the **exact** telemetry, sensor confidence, Doppler speed, and visual conditions available at that precise moment without revealing post-event ground truth.

### 6. Closed-Loop Adaptive Training Curriculum
The platform evaluates trainee performance across detection latency, classification accuracy, and escalation decisions. When sensor uncertainty weaknesses are detected, the system autonomously synthesizes adaptive drills targeting those specific failure modes.

---

## 🚀 Quick Start Guide

### Prerequisites
* Any modern web browser with WebGL hardware acceleration enabled (Chrome, Edge, Firefox, Safari).
* Python 3.x (optional, for local hosting).

### Running Locally

```bash
# 1. Clone the repository
git clone https://github.com/Jacksonfio/drone.git
cd drone

# 2. Start a local HTTP server
python -m http.server 3000

# 3. Open your browser
# Navigate to: http://localhost:3000
```

Alternatively, open `index.html` directly in your web browser.

---

## 🎮 Interactive Controls

| Input | Action |
|---|---|
| **Left Click + Drag** | Look around / Rotate observer camera viewpoint |
| **Right Click + Drag** | Pan camera position across battlespace |
| **Mouse Scroll Wheel** | Adjust camera zoom / dolly |
| **Quick Zoom Buttons (+ / -)** | Step optical PTZ magnification (1.0x - 8.0x) |
| **1-Click Drone Focus Button** | Instantly snap and zoom camera onto active drone |
| **Terrain Buttons** | Switch between City, Mountain, Village, and Port |
| **Drone Type Selector** | Switch between Quadcopter, Fixed-Wing, Hexacopter, and FPV |
| **Weather Toggles** | Switch between Day, Night, Fog, and Rain |
| **Trainee Action Bar** | Classify threat (`DRONE`, `NON-THREAT`, `UNKNOWN`) and dispatch response (`MONITOR`, `VERIFY`, `ALERT`) |

---

## 📁 Repository Structure

```text
├── index.html          # Complete THREATVERSE single-page simulation platform
├── three.min.js        # Three.js WebGL 3D rendering engine (r128)
├── OrbitControls.js    # 3D camera pan, rotate, and zoom controller
└── README.md           # Master documentation and deployment guide
```

---

## 🛡️ Operational Philosophy

> **REAL WORLD → SIMULATED SAFELY → MEASURED → REPLAYED → EXPLAINED → ADAPTED**

THREATVERSE is strictly an assessment, simulation, and educational trainer designed to build rapid visual recognition and measured decision-making under high-stress, degraded-sensor operational conditions.

---

## 👤 Author & Maintainer
* **Repository:** [https://github.com/Jacksonfio/drone](https://github.com/Jacksonfio/drone)
* **Author:** Jackson Fio (`jacksonjp646@gmail.com`)
