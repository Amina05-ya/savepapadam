<img width="1280" height="640" alt="git (1)" src="https://github.com/user-attachments/assets/8920b256-2ba8-4988-b824-5351134eb4bd" />



# [pappadamguard] 🎯


## Basic Details
### Team Name: [peak nonsense]


### Team Members
- Team Lead: [Amina S] - [COLLEGE OF ENGINEERING PERUMON]
- Member 2: [Anamika V S] - [COLLEGE OF ENGINEERING PERUMON]


### Project Description
### PappadamGuard 🛡️🍘

PappadamGuard is a fun IoT-based security and monitoring system for pappadam. It uses **RFID authentication, IR sensing, servo control, LEDs, buzzer, and LCD** for access control, while "Python and OpenCV"analyze the pappadam through a phone camera and estimate its crack/damage percentage.

"Tech Stack:"Arduino UNO, RC522 RFID, Python, OpenCV, IoT, Computer Vision.


### The Problem (that doesn't exist)
[What ridiculous problem are you solving?]
People stealing, touching, or damaging one precious pappadam without permission.

PappadamGuard solves this “critical” problem using RFID authentication, IR sensing, a servo-controlled cover, buzzer alerts, LCD messages, and camera-based crack detection.


### The Solution (that nobody asked for)
[How are you solving it? Keep it fun!]
PappadamGuard uses RFID to identify the owner, an IR sensor to detect intruders, and a servo motor to open the pappadam’s VIP cover. A buzzer scares away unauthorized snack thieves, while a camera and Python detect cracks and calculate the pappadam’s “damage percentage.”


## Technical Details
### Technologies/Components Used
For Software:
- [Languages used]
- [Frameworks used]
- [Libraries used]
- [Tools used]
For Software:

* Languages used: Python, C/C++ (Arduino)

* Frameworks used: Arduino Framework, OpenCV

* Libraries used:

  * OpenCV

  * NumPy

  * PySerial

  * SPI

  * MFRC522

  * LiquidCrystal_I2C

  * Servo

* Tools used: Arduino IDE, Python IDLE/VS Code, DroidCam, Arduino UNO, USB Serial Communication

For Hardware:
- [List main components]
- [List specifications]
- [List tools required]
### For Hardware

* Main components:

  * Arduino UNO

  * RC522 RFID Reader and RFID Card

  * 16×2 I2C LCD Display

  * IR Proximity Sensor

  * SG90 Servo Motor

  * Buzzer

  * Red LED and Green LED

  * Resistors

  * Breadboard and Jumper Wires

  * Mobile Phone/Webcam for crack detection

* Specifications:

  * Arduino UNO: ATmega328P, 5V operating voltage

  * RC522 RFID: 13.56 MHz, 3.3V operating voltage, SPI communication

  * LCD: 16×2 characters, I2C communication, usually address `0x27`

  * IR Sensor: Digital proximity detection, 5V supply

  * SG90 Servo: 5V, approximately 0°–180° rotation

  * Buzzer: 5V active buzzer for alert sounds

  * LEDs: 5mm red and green LEDs with 220Ω resistors

  * Webcam: Used to capture the pappadam and detect cracks using Python/OpenCV

  * Communication: USB serial communication between Arduino and computer

* Tools required:

  * Arduino IDE

  * USB cable

  * Breadboard

  * Jumper wires

  * Screwdriver

  * Wire cutter/stripper

  * Laptop or computer

  * Mobile phone with DroidCam or a webcam

  * Soldering iron (optional, for permanent connections)

### Implementation
For Software:
# Installation
[commands]
Install Python and the required libraries using Command Prompt:

Bash

```
python --version
```

Bash

```
pip install opencv-python
pip install numpy
pip install pyserial
```

Install the following software tools:

* Arduino IDE

* Python 3

* OpenCV

* NumPy

* PySerial

* DroidCam (if using a mobile phone as a webcam)

For DroidCam, install the mobile application and the Windows client, then connect the phone camera to the laptop.

Arduino IDE libraries required:

* MFRC522

* LiquidCrystal_I2C

* Servo

* SPI

* Wire

These libraries can be installed through:

```
Arduino IDE → Sketch → Include Library → Manage Libraries
```

After installation:

1. Upload the Arduino code using Arduino IDE.

2. Check the correct Arduino COM port.

3. Update the COM port in the Python code.

4. Run the Python program.

5. Use the webcam to detect the pappadam and calculate its damage percentage.

# Run
[commands]
Bash

```
python pappadamguard.py
```

If using Python IDLE:

1. Open `pappadamguard.py`

2. Click Run

3. Select Run Module or press F5

Before running, ensure:

Bash

```
pip install opencv-python numpy pyserial
```

Also check:

* Arduino is connected.

* Correct COM port is used in the Python code.

* DroidCam is running.

* Close Arduino Serial Monitor before running Python.


### Project Documentation
For Hardware:

# Schematic & Circuit
RFID Card → Arduino UNO → Authentication → Servo Lock → IR/Ultrasonic Detection → Camera → Crack/Damage Detection → Buzzer + LCD + LED
Caption:

Figure 1: Overall workflow of PappadamGuard showing RFID-based access control, sensor monitoring, servo-based protection, and camera-based pappadam damage detection.
  file:///C:/Users/HP/OneDrive/Documents/schematic.pdf
  

# Build Photos
![Components](Add photo of your components here)
*List out all components shown*
"C:\Users\HP\OneDrive\Documents\COMPONENTS.png"
Arduino UNO
RC522 RFID module
16×2 I2C LCD
Servo motor
IR sensor
Red LED
Green LED
Buzzer
Power supply

![Build](Add photos of build process here)
"C:\Users\HP\OneDrive\Documents\papad building.mp4"
"C:\Users\HP\OneDrive\Documents\building2.mp4"
*Explain the build steps*
The build process started by assembling the Arduino UNO, RC522 RFID reader, I2C LCD, IR sensor, servo motor, buzzer, LEDs, and other components on a breadboard. The RFID reader, LCD, and sensors were connected to the Arduino according to the circuit design. The servo motor was attached to the protective cover. The Arduino code was uploaded using Arduino IDE and tested for RFID access, LED indications, buzzer alerts, LCD messages, and servo movement. Finally, a phone camera connected through DroidCam was integrated with the Python OpenCV program to detect pappadam cracks and calculate the damage percentage.


![Final](Add photo of final product here)
*Explain the final build*
"C:\Users\HP\OneDrive\Documents\pappad.jpeg"
"C:\Users\HP\OneDrive\Documents\pappad2.jpeg"
The final build is a compact smart security system designed to protect a pappadam. When a person approaches, the IR sensor activates the system and the user must scan an authorized RFID card. If the card is valid, the green LED glows, the buzzer gives a confirmation sound, and the servo motor opens the protective cover. If an unauthorized card is detected, the red LED and buzzer indicate access denial. The LCD displays system messages and the estimated pappadam damage percentage received from the Python OpenCV camera system.


### Project Demo
# Video
[Add your demo video link here]
"C:\Users\HP\OneDrive\Documents\papad video.mp4"
### Brief Idea of the Project

PappadamGuard is a fun smart security and monitoring system designed to protect a pappadam from unauthorized access and damage. It uses an RFID card for authentication, an IR sensor to detect approaching users, and a servo motor to open or close the protective cover. LEDs, a buzzer, and an LCD provide status messages and alerts. A phone camera with Python and OpenCV detects cracks in the pappadam and displays the estimated damage percentage.

# Additional Demos
[Add any extra demo materials/links]

## Team Contributions
- [Amina S]: :project idea, Python programming, OpenCV-based crack detection, and camera integration,testing, documentation, and presentation.
- [Anamika V S]: Arduino programming, RFID authentication, and servo motor control,Circuit assembly, LCD/LED/buzzer integration.


---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProjects--26-26?link=https%3A%2F%2Ftinkerhub.org%2Fevents%2F1M8ORET9A1%2Fuseless-projects-3.0)



