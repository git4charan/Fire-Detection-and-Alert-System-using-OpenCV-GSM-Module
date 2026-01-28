# Python – Fire Detection Module 

This folder contains the **computer vision and alerting logic** for detecting fire using a live camera feed.

---

## Files
- `fire_detection.py`  
  Main Python script responsible for:
  - Capturing video feed
  - Detecting fire using Haar Cascade
  - Playing alarm sound
  - Sending email alerts
  - Communicating with Arduino via serial

- `fire_detection_cascade_model.xml`  
  Pre-trained Haar Cascade classifier used for fire detection.

- `fire_alarm.mp3`  
  Audio file played when fire is detected.

---

## How It Works
1. Camera feed is captured using OpenCV
2. Each frame is analyzed for fire patterns
3. If fire is detected:
   - Alarm sound is played using threading
   - Email alert is sent (only once per session)
   - Signal is sent to Arduino via serial port

---

##  Configuration Required
Before running:
- Update `COM` port in `fire_detection.py`
- Replace email credentials with valid values
- Ensure required Python libraries are installed:
  - `opencv-python`
  - `playsound`
  - `pyserial`

---

##  Notes
- Email credentials are intentionally left as placeholders
- Cascade model is used as-is for detection
- Script exits when `q` is pressed
