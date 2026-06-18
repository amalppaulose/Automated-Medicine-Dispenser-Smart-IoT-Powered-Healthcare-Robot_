# Automated-Medicine-Dispenser-Smart-IoT-Powered-Healthcare-Robot_
Elderly and chronically ill patients often miss medications due to lack of assistance. Existing dispensers are stationary — patients still have to walk to them. We eliminated that dependency entirely.
What We Built
An autonomous, cloud-connected medicine dispensing robot that:

Navigates autonomously to the patient's bedside using IR line-follower sensors
Dispenses up to 4 different medicines at scheduled times via servo-controlled 3D-printed containers
Serves water automatically through an integrated mini pump
Sends real-time refill alerts when medicine runs low (photoelectric sensors)
Returns to its docking position automatically after dispensing
Is controlled remotely from anywhere in the world via the Blynk IoT app

Architecture
Blynk Cloud (Schedule & Dosage)
        ↓
      ESP32 (WiFi + Logic)
        ↓
   Arduino UNO (Motor Control)
    ↙          ↘
IR Sensors    L298N Motor Driver
(Navigation)      ↓
            4× DC Motors (Rover)
            4× Servo Motors (Dispensers)
            Water Pump

Key Hardware
ESP32, Arduino UNO,SG90 Servo × 4P, IR Sensors, Photoelectric Sensor, Li-ion Pack (11.1V, 6.6A)Portable power with BMS protection, R385 Mini Pump

Innovation Highlights
The dispenser container is angled at 35.5° — a deliberate design choice ensuring pills accumulate only on the dispensing side, preventing accidental multi-pill drops. The rotating base (23mm opening, 2mm thick) was precision-modelled in Fusion 360 and 3D-printed.
No manual intervention needed — from scheduling on your phone to medicine arriving at your bedside, the entire pipeline is automated.

User Experience
Through the Blynk app you can:
Set morning / noon / night dosage for each of 4 medicines
Monitor container levels visually in real-time
Trigger manual dispensing remotely
Receive push notifications when medicine needs refilling

Built for ₹20,526
Proving that life-improving medical robotics doesn't require a Fortune 500 budget.

Future Roadmap
Syrup dispensing module
Vitals monitoring (SpO2, BP)
SOS signal to nearest health centre
LED touchscreen interface
Wireless charging dock
Multi-patient deployment (hospital wards)
