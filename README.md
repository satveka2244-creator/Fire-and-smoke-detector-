🔥 Fire and Smoke Detector using Arduino UNO

A Low-Cost Fire and Smoke Detection System

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Arduino%20UNO-blue">
  <img src="https://img.shields.io/badge/Language-Embedded%20C-green">
  <img src="https://img.shields.io/badge/Project-ECE-orange">
  <img src="https://img.shields.io/badge/Status-Prototype-yellow">
</p>---

📌 Project Overview

Fire accidents are a major threat to human life and property in residential, commercial, and industrial environments.

Delayed detection of fire and smoke can lead to serious damage and dangerous situations. Traditional fire safety systems may require expensive equipment or depend on human observation.

To address this problem, this project presents a low-cost, Arduino-based Fire and Smoke Detector System that continuously monitors the surrounding environment using smoke and flame sensors.

The system uses an Arduino UNO microcontroller, MQ-2 smoke sensor, flame sensor, buzzer, LED indicators, and LCD display.

When smoke or flame is detected, the Arduino processes the sensor signals and activates an alarm to alert nearby people.

The project focuses on:

- Early detection of fire and smoke.
- Real-time environmental monitoring.
- Automatic audible and visual alerts.
- Low-cost implementation.
- Simple installation and operation.
- Improving awareness of fire safety.

---

🎯 Objectives

The main objectives of this project are:

- To detect smoke and flames in real time.
- To develop a low-cost fire safety system.
- To continuously monitor the surrounding environment.
- To activate a buzzer when fire or smoke is detected.
- To provide visual alerts using LED indicators.
- To display system status through an LCD.
- To reduce the delay in identifying fire hazards.
- To improve safety in homes, offices, schools, and industries.
- To demonstrate the application of sensors and microcontroller technology.
- To provide a foundation for future IoT-based fire monitoring systems.

---

✨ Features

- 🔥 Flame detection using a flame sensor module.
- 🌫️ Smoke and gas detection using an MQ-2 sensor.
- 🚨 Automatic buzzer activation.
- 💡 LED-based visual indication.
- 📟 LCD display for system status.
- ⚡ Arduino UNO-based control.
- 🔄 Continuous sensor monitoring.
- 💰 Low-cost hardware implementation.
- 🏠 Suitable for residential and educational environments.
- 📡 Potential for future IoT integration.

---

🛠️ Hardware Components

S.No| Component| Purpose
1| Arduino UNO| Main microcontroller
2| MQ-2 Smoke/Gas Sensor| Detects smoke and combustible gases
3| Flame Sensor Module| Detects visible flame
4| Buzzer| Provides audible warning
5| LED Indicators| Provides visual warning
6| 16×2 LCD Display| Displays system status
7| Breadboard| Circuit construction
8| Jumper Wires| Electrical connections
9| DC Power Supply| Powers the system

---

💻 Software Requirements

Software| Purpose
Arduino IDE| Writing and uploading Arduino code
Embedded C| Programming the microcontroller
Circuit Simulation Software| Circuit design and simulation
Sensor Datasheets| Understanding sensor specifications

---

⚙️ Working Principle

The Fire and Smoke Detector System works by continuously monitoring the surrounding environment.

Step 1: Environmental Monitoring

The MQ-2 smoke sensor monitors smoke and gas concentrations.

The flame sensor module detects the presence of visible flames.

Step 2: Sensor Input

The sensors provide signals to the Arduino UNO.

Step 3: Data Processing

The Arduino processes the sensor signals and checks whether smoke or flame has been detected.

Step 4: Alarm Activation

When a hazardous condition is detected:

- The buzzer is activated.
- The LED indicator provides a visual warning.
- The LCD displays the detected condition.

Step 5: Normal Operation

When no smoke or flame is detected, the system continues monitoring the environment.

---

🔄 System Workflow

flowchart TD
    A([Start]) --> B[Initialize Arduino]
    B --> C[Initialize Sensors]
    C --> D[Initialize LCD and Alarm]
    D --> E[Monitor Smoke Sensor]
    E --> F[Monitor Flame Sensor]
    F --> G{Smoke or Flame Detected?}
    G -->|No| H[Display Normal Status]
    H --> E
    G -->|Yes| I[Activate Buzzer]
    I --> J[Activate LED]
    J --> K[Display Fire or Smoke Alert]
    K --> E

---

🔌 Circuit Connections

The circuit connects the sensors and output devices to the Arduino UNO.

Main Connections

Component| Connection
MQ-2 Smoke Sensor| Arduino input
Flame Sensor| Arduino input
Buzzer| Arduino output
LED Indicator| Arduino output
LCD Display| Arduino display interface
Power Supply| Arduino and sensor power
Ground| Common circuit ground

Note: Refer to the circuit diagram included in the project report for the exact pin connections.

The pin numbers should be added according to the actual circuit used in the prototype.

---

🧠 System Architecture

The system consists of three major sections.

1. Input Section

The input section includes:

- MQ-2 smoke sensor.
- Flame sensor module.

These sensors continuously monitor the surrounding environment.

2. Processing Section

The Arduino UNO acts as the central processing unit.

It:

- Reads sensor signals.
- Processes sensor inputs.
- Identifies hazardous conditions.
- Controls the output devices.

3. Output Section

The output section includes:

- Buzzer.
- LED indicators.
- LCD display.

These devices provide audible, visual, and display-based alerts.

---

📊 Sample Output

Normal Condition

System Active
No Fire/Smoke Detected

Smoke Detection

Smoke Detected
Buzzer Activated
LED Alert

Flame Detection

Fire Detected
Buzzer Activated
LED Alert

Combined Detection

Fire and Smoke Detected
Emergency Alert

The displayed messages are illustrative. Actual LCD messages depend on the Arduino program.

---

🚀 Installation and Setup

Step 1: Collect Components

Collect the Arduino UNO, MQ-2 sensor, flame sensor, buzzer, LED, LCD, breadboard, and jumper wires.

Step 2: Assemble the Circuit

Connect the sensors and output devices to the Arduino UNO according to the circuit diagram.

Step 3: Install Arduino IDE

Download and install the Arduino IDE.

Official website:

https://www.arduino.cc/en/software

Step 4: Prepare the Arduino Code

Create an Arduino sketch and implement the sensor monitoring and alarm logic.

Step 5: Connect Arduino

Connect the Arduino UNO to the computer using a USB cable.

Step 6: Select Board

In Arduino IDE:

1. Open Tools.
2. Select Board.
3. Choose Arduino UNO.
4. Select the appropriate COM port.

Step 7: Upload the Program

Upload the Arduino program to the board.

Step 8: Test the System

Check the sensor readings, LCD display, buzzer, and LED indicators under controlled conditions.

---

📁 Project Structure

Fire-and-Smoke-Detector/
│
├── README.md
│
├── Arduino-Code/
│   └── fire_smoke_detector.ino
│
├── Circuit-Diagram/
│   └── circuit_diagram.png
│
├── Block-Diagram/
│   └── block_diagram.png
│
├── Flowchart/
│   └── system_flowchart.png
│
├── Images/
│   └── prototype.jpg
│
├── Documentation/
│   └── project_report.pdf
│
└── LICENSE

Add the corresponding files and folders to your repository as you create them.

---

🧪 Testing and Results

The prototype was tested under controlled conditions to evaluate its detection and alert functions.

Smoke Detection Test

The MQ-2 sensor was used to monitor smoke and gas emissions.

When the sensor detected a hazardous condition, the Arduino processed the input and activated the alert system.

Flame Detection Test

The flame sensor module was used to identify visible flames.

When flame detection occurred, the Arduino activated the buzzer and LED indicators.

Alarm Test

The buzzer and LED indicators were checked to confirm that the alert system responded to sensor inputs.

LCD Test

The LCD display was used to provide information about the system condition.

Overall Result

The prototype demonstrated the basic operation of an Arduino-based fire and smoke detection system.

The system provides:

- Sensor-based monitoring.
- Automatic alarm activation.
- Visual indication.
- LCD status display.
- Low-cost implementation.

The prototype is intended for educational demonstration and further development.

---

🏠 Applications

The Fire and Smoke Detector System can be used as an educational prototype for:

Residential Buildings

Provides an early warning of smoke and fire hazards.

Offices

Supports fire safety awareness and environmental monitoring.

Educational Institutions

Can be demonstrated in classrooms, laboratories, and project exhibitions.

Industrial Environments

Demonstrates the use of sensors for monitoring fire-related hazards.

Warehouses

Can be developed for monitoring smoke and flame conditions.

Smart Buildings

Can be extended with wireless communication and remote monitoring.

---

⚠️ Limitations

The current prototype has the following limitations:

- The MQ-2 sensor requires calibration.
- Sensor readings may be affected by environmental conditions.
- The detection range depends on sensor placement.
- Larger areas require additional sensors.
- The system depends on a continuous power supply.
- The current implementation provides local alarms.
- Remote monitoring requires additional communication hardware and software.
- The prototype is not a certified fire safety system.

---

🔮 Future Scope

The project can be improved by integrating additional technologies.

1. IoT Integration

Connect the system to an IoT platform for remote monitoring.

2. GSM Communication

Integrate a GSM module to send SMS alerts to registered users.

3. Wireless Sensor Network

Use multiple wireless sensors to monitor larger environments.

4. Temperature Monitoring

Add a temperature sensor to improve environmental monitoring.

5. Cloud Monitoring

Store sensor readings and event information on a cloud platform.

6. Smart Building Integration

Integrate the system with building monitoring and automation systems.

7. Improved Detection Accuracy

Explore sensor calibration and intelligent processing to improve reliability.

---

👥 Project Team

Department: Electronics and Communication Engineering

Institution: KPR Institute of Engineering and Technology, Coimbatore

Team Members

S.No| Name| Register Number
1| Sudharson V| 25EC230
2| Sanjay Sudha Periyasamy| 25EC194
3| Saranya S| 25EC204
4| Satveka A| 25EC206

Project Guidance

Department of Physics

KPR Institute of Engineering and Technology

---

📚 References

1. Arduino Official Documentation
   https://docs.arduino.cc/

2. Arduino IDE
   https://www.arduino.cc/en/software

3. MQ-2 Smoke and Gas Sensor Datasheet.

4. Flame Sensor Module Documentation.

5. Project Report: Fire and Smoke Detector.

---

🛡️ Safety Disclaimer

This project is an educational prototype developed for academic purposes.

It is not a certified fire detection or life-safety device and must not replace approved smoke alarms, fire alarm systems, or professional fire safety equipment.

All testing should be performed under appropriate supervision and in a safe, controlled environment.

---

📄 License

This project is intended for educational and academic use.

A license has not yet been selected. Add a "LICENSE" file if you intend to publish the project with specific reuse permissions.

---

⭐ Acknowledgment

We express our sincere gratitude to our institution, project coordinators, faculty members, and everyone who supported the development of this project.

This project helped us understand the practical application of sensors, microcontrollers, embedded programming, and electronic circuit design.

---

<p align="center">
  <b>🔥 Fire and Smoke Detector using Arduino UNO 🔥</b>
  <br>
  Electronics and Communication Engineering
</p>
