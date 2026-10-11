# AI-Assisted Smart Blind Stick

**HackFest 2026 | Team-5A.11**

## 1. Project Overview

The AI-Assisted Smart Blind Stick is an assistive technology prototype designed to help visually impaired people identify nearby obstacles and understand their surroundings through computer vision, distance sensing, and voice feedback.

The system uses a Raspberry Pi, a camera, an AI-based object detection model, and an ultrasonic sensor to provide audio and visual alerts.

## 2. Problem Statement

Conventional walking sticks help users detect physical obstacles through contact but cannot independently identify objects or provide detailed spoken information about the surroundings.

This project explores how AI and electronic sensors can improve environmental awareness and support safer, more informed mobility.

## 3. Proposed Solution

The proposed system combines camera-based object detection with ultrasonic distance sensing.

- The camera captures the surrounding environment.
- The YOLO model identifies supported objects.
- The ultrasonic sensor estimates the distance to nearby obstacles.
- The controller prioritizes obstacle warnings using programmed decision logic.
- Voice feedback, a buzzer, and an LED provide alerts to the user.

## 4. Key Features

- AI-based object detection.
- Ultrasonic obstacle-distance sensing.
- Voice announcements using eSpeak NG.
- Buzzer and LED alerts for nearby obstacles.
- Raspberry Pi-based processing.
- Integration of camera and sensor inputs.

## 5. Hardware Requirements

- Raspberry Pi 3B+ or compatible Raspberry Pi board.
- Compatible Raspberry Pi camera module.
- Ultrasonic distance sensor.
- LED and suitable current-limiting resistor.
- Compatible buzzer and required interface components.
- Power supply, jumper wires, and mounting structure.

## 6. Software and Technologies

- Python
- Raspberry Pi GPIO
- Picamera2
- Ultralytics YOLO
- OpenCV
- NumPy
- eSpeak NG

## 7. System Architecture

**Camera → YOLO Object Detection → Decision Logic → Voice Feedback**

**Ultrasonic Sensor → Distance Estimation → Obstacle Alert Logic → Buzzer and LED**

The decision logic prioritizes nearby obstacle warnings over routine object announcements.

## 8. Repository Structure

- `main.py` — Main application code.
- `requirements.txt` — Python package dependencies.
- `3D-Model.png` — Mechanical design model.
- `Circuit-Diagram.png` — Circuit diagram.
- `Final-Product.png` — Prototype photograph.
- Demonstration videos — Recorded prototype demonstrations.

## 9. Implementation Plan

1. Assemble and verify the hardware connections.
2. Test camera capture and object detection.
3. Test ultrasonic distance measurement.
4. Integrate voice announcements and obstacle alerts.
5. Test the integrated prototype under different conditions.
6. Document results, limitations, and future improvements.

## 10. Testing and Evaluation

The integrated system will be evaluated using:

- Object detection performance under different lighting conditions.
- Distance measurement accuracy at different ranges.
- Response time for obstacle alerts.
- Reliability of voice and buzzer feedback.
- Overall system stability during continuous operation.

Actual measurements and results will be added after testing.

## 11. Current Limitations

- Object detection depends on lighting, camera quality, and model performance.
- Ultrasonic sensing has limitations related to surface shape, angle, and range.
- The current implementation does not provide comprehensive stair or drop-off detection.
- The system does not independently plan a safe walking route.

## 12. Future Enhancements

- Dedicated stair and drop-off detection.
- Improved context-aware hazard prioritization.
- Better sensor fusion and reduced repeated announcements.
- GPS-based location assistance.
- Emergency notification features.
- Improved power efficiency and usability.

## 13. Safety Disclaimer

This prototype is intended for research and demonstration. It is not a replacement for a conventional white cane, guide dog, or professional mobility training. Users must not rely on the system as their sole means of detecting hazards.

## 14. Project Status

**Status:** Prototype development and integration.

Testing results, verified performance measurements, and additional implementation details will be updated as development progresses.
