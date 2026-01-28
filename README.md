# Fire-Detection-and-Alert-System-using-OpenCV-GSM-Module


A real-time fire detection and alerting system built using **OpenCV (Python)** and **Arduino with GSM**, developed as an academic project and later organized for reproducibility and demonstration.

---

## Project Overview
The system uses a camera feed to detect fire using computer vision.  
Once fire is detected, it triggers:
- An audible alarm
- Email notification
- Arduino-based alerting (buzzer, LEDs, relay)
- SMS and call alerts via GSM module

---

## Technologies Used
- Python (OpenCV, threading, serial communication)
- Haar Cascade Classifier (XML model)
- Arduino (LCD, GSM, relay, buzzer)
- Serial communication (USB)
- SMTP (email alerts)

---


---

## How the System Works
1. Camera captures live video feed
2. Fire is detected using a Haar Cascade classifier
3. Alarm sound is played
4. Email alert is sent (once per detection)
5. Arduino receives signal via serial communication
6. GSM module sends SMS and initiates a call

---

## Hardware Components
- Arduino UNO
- GSM Module
- Buzzer
- LEDs
- Relay Module
- LCD Display
- Camera (Laptop / USB)

---

## Configuration Notes
- Email credentials in Python code are placeholders
- COM port must be updated as per system
- Phone numbers must be configured in Arduino code
- Project is intended for demonstration and learning purposes

---

## Future Improvements
- CCTV camera integration
- Mobile app or cloud notifications
- Improved fire detection model (CNN / YOLO)
- Remote monitoring dashboard

