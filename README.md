# 🤖 LUXI: The AI Companion Bot (3D-Printed & Local)

## Project Overview

Status: **Just an idea and some models so far**
Funding: **Fingers crossed for a Hack Club Blueprint grant!** (Asking for $400)
Languages: **Python, MicroPython**

Luxi's gonna be a small, kinda sassy, roving robot buddy. We're printing all the parts and want it to run locally for speed and, you know, privacy.

What makes Luxi cool is the way it's built. The PC handles the heavy AI lifting and talking stuff, while the ESP32 controls the robot's body in real-time kinda via Wi-Fi.

### ⚙️ What it's made of

Everything's designed to be 3D-printed to keep costs down and make the most of the printer.

* **3D-Printed Body:** Body, wheels, and stuff are getting printed on an Anycubic Kobra 3 V2.

* **Expressive Head:** Servos make the head turn and tilt like it's listening.

* **Light-Up Eyes and Moods:**

* **OLED Eyes:** Little screens show animated faces.

* **Mood Light:** RGB LEDs (WS2812B) show if it's ready, listening, or talking back.

* **Charging Dock:** A printed dock with a TP4056 thingy to charge the battery safely.

### 💻 How it Works (Software)

We're planning to use a solid **WebSocket** setup to keep the PC and robot talking to each other quickly.

* **PC (Brain) - Python:**

* **What it does:** Runs the AI, figures out what to say and hears what you say.

* **How It Works:** Sends commands to the robot in the form of JSON.

* **ESP32 (Body) - MicroPython:**

* **What it does:** Gets the JSON from the PC.

* **How It Works:** Moves the motors, servos, and shows stuff on the screens.
