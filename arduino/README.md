# Arduino – Fire Alert System 

This folder contains the Arduino code responsible for **physical alerting and GSM communication**.

---

## File
- `fire_alert_system.ino`  
  Controls:
  - LCD display messages
  - Buzzer and LED indicators
  - Relay activation
  - GSM-based SMS and call alerts

---

## How It Works
1. Arduino listens for serial input from Python
2. On receiving:
   - `'F'` → Fire detected
     - Activates buzzer, LED, relay
     - Sends SMS with location
     - Makes an emergency call
   - `'S'` → No fire
     - Resets system to normal state

---

## Hardware Connections
- LCD connected using `LiquidCrystal` library
- GSM module connected via serial
- Buzzer, LEDs, and relay connected to analog pins

---

## Configuration Required
- Update phone number in GSM commands
- Ensure GSM module is powered properly
- SIM card must support SMS and calling

---

## Notes
- Uses AT commands for GSM communication
- Designed for academic and demonstration purposes
