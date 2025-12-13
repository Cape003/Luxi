# LUXI: The AI Companion Bot (3D-Printed & Local)

## Project Overview

Luxi's gonna be a small, kinda sassy, roving robot buddy. We're printing all the parts and want it to run locally for speed and, you know, privacy.

What makes Luxi cool is the way it's built. The PC handles the heavy AI lifting and talking stuff, while the ESP32 controls the robot's body in real-time kinda via Wi-Fi.

### Why am I doing this?

My project, LUXI, stems from two desires: to create something cool and tangible, and to explore electronics.

It's more than just a robot; it's my playground for learning. I really want to make significant progress on the hardware side. The idea is to manage the entire robot creation cycle: from 3D design to printing, including wiring and microcontroller programming.

By building Luxi, I'll learn to use a wide variety of electronic components. It's fantastic, and above all, I'm learning a ton!

Luxi is a perfect platform for practicing the integration of software (Python and AI) and hardware. With this funding, I could truly transform this project into a real educational experience, creating a small, expressive, and technically advanced robot that is, frankly, incredibly interesting.

### What it's made of

Everything's designed to be 3D-printed to keep costs down and make the most of the printer.

* **3D-Printed Body:** Body, wheels, and stuff are getting printed on an Anycubic Kobra 3 V2.

* **Expressive Head:** Servos make the head turn and tilt like it's listening.

* **Light-Up Eyes and Moods:**

* **OLED Eyes:** Little screens show animated faces.

* **Mood Light:** RGB LEDs (WS2812B) show if it's ready, listening, or talking back.

* **Charging Dock:** A printed dock with a TP4056 thingy to charge the battery safely.

### How it Works (Software)

We're planning to use a solid **WebSocket** setup to keep the PC and robot talking to each other quickly.

* **PC (Brain) - Python:**

* **What it does:** Runs the AI, figures out what to say and hears what you say.

* **How It Works:** Sends commands to the robot in the form of JSON.

* **ESP32 (Body) - MicroPython:**

* **What it does:** Gets the JSON from the PC.

* **How It Works:** Moves the motors, servos, and shows stuff on the screens.
