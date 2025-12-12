# 🤖 LUXI: The AI Companion Bot (3D-Printed & Local)

| **Project Status** | **Funding** | **Target Languages** |

|:--- |:--- | :--- |

| **Concept & Modelling** | **Submission Hack Club Blueprint in Progress** | **Python, MicroPython** |

### ✨ Project Overview

**Luxi** is a miniature, expressive and mobile companion robot, entirely designed from **3D printed pieces**. The goal is to create a single physical terminal for an intelligent dialogue system, favouring a **local architecture** for speed and privacy.

The originality of Luxi lies in its hybrid architecture: it separates the complex processing of **Artificial Intelligence (AI) and dialogue** (managed by a Large Language Model on a PC) from **real-time physical control** (managed by the ESP32 microcontroller via Wi-Fi).

### ⚙️ Technical Characteristics

Each structural component is designed to be custom-made, which maximises the use of 3D printing.

* **Customised 3D Structure:** The body, chassis, engine mounts and even **functional wheels** are 3D printed, ensuring the robustness and unique aesthetics of the robot.

* **Expressive Control:** Head Mechanism (Pan/Tilt) controlled by servomotors to simulate listening.

* **Visual Feedback (Light):**

* **OLED eyes:** Two screens display animated facial expressions.

* **Humour Indicator:** RGB LEDs (WS2812B) signal the status (ready, listening, response).

* **Optimised Charging Station:** A custom 3D printed dock integrating the TP4056 module for secure charging of the LiPo battery.

### 💻 Software Architecture 

Programming will focus on establishing a stable **WebSocket** protocol for real-time communication and task decomposition between the two systems.

| System | Role | Target Language |

|:--- |:--- | :--- |

| **PC (Master)** | **Intelligence & Dialogue:** Executes local LLM, manages vocal recognition/synthesis. Sends action commands (JSON) to the robot. | **Standard Python** |

| **ESP32 (Client)** | **Physical Control:** Receives the JSON message from the PC, decodes it, and directly controls the engines, servos, and displays. |**MicroPython**|


### 🎯 Next Steps (Roadmap)

* [x] Finalisation of the Concept, BOM and Wiring Diagram.

* [ ] **3D modelling:** Design of the Luxi body, wheels, and charging station.

* [ ] Acquisition of equipment (After receipt of Blueprint funding).

* [ ] Development of MicroPython and Python firmwares.

* [ ] Assembly, wiring, and software integration.

---

