# Pixy2 Pan-Tilt Servo Control (Arduino)

This Arduino project uses the **Pixy2 CMUcam5** with its **Pan-Tilt Servo Kit** to track user-defined objects in real time. The Pixy2 is trained to recognize specific color signatures, and the servos automatically adjust to center the selected object within its field of view.

## 🛠️ Requirements

- Pixy2.1
- Pixy2 Pan-Tilt Kit
- Arduino-compatible board
- Pixy2 Arduino Library

## 🎯 Features

- Tracks **custom-trained object signatures** (set via PixyMon)
- Automatically adjusts **pan** and **tilt** servos to follow the object
- Suitable for turrets, interactive displays, or educational robotics

## ⚙️ Setup Instructions

1. **Train objects** in PixyMon by assigning color signatures (e.g., Sig1, Sig2)
2. Upload the example sketch from Pixy2 library:  
   `File > Examples > Pixy2 > pan_tilt_demo`
3. Or use the custom sketch included in this repo.
4. Ensure servos are connected to Pixy2’s built-in servo headers (pan = servo0, tilt = servo1)
   
![image](https://github.com/user-attachments/assets/3858ebc0-39c6-4d32-aa18-0cb913fc25da)
![image](https://github.com/user-attachments/assets/c406d1b2-0cbe-42bb-86ef-f57890937b4c)

## 🧠 Notes

- You can train and store multiple color signatures (Sig1–Sig7)
- Use `pixy.setServos(pan, tilt)` to manually adjust servo angles (range: 0–1000)
- Pixy2 handles object detection and tracking directly on the sensor

## 📚 Library Installation

Install the Pixy2 Arduino Library via:
- Arduino IDE > **Library Manager**
- Or from the [[official GitHub repo](https://github.com/charmedlabs/pixy2](https://pixycam.com/downloads-pixy2/))


