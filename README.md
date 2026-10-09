# 📡 Arduino-Based Ultrasonic Radar System

A simple electronics project that uses an **Arduino Uno, an ultrasonic sensor, and a servo motor** to scan the surrounding area and detect nearby objects based on distance measurements.

This project was built to explore basic robotics, sensor interfacing, servo motor control, and real-time distance measurement using Arduino.

## 📌 Project Overview

The system rotates an ultrasonic sensor using a servo motor, allowing it to measure distances at different angles. The Arduino processes the sensor readings and can be used to display the detected object's angle and distance.

This project is a beginner-friendly introduction to combining hardware components with embedded C/C++ programming.

> **Note:** This is an ultrasonic scanning system inspired by radar, not a conventional radio-frequency radar.

## ✨ Features

- 📏 Measures the distance to nearby objects using an ultrasonic sensor.
- 🔄 Rotates the sensor using a servo motor to scan different angles.
- 🎯 Associates distance measurements with the sensor's scanning angle.
- ⚡ Uses an Arduino Uno for sensor reading and motor control.
- 🛠️ Built using accessible electronic components.
- 📚 Demonstrates fundamental embedded systems concepts.

## 🧰 Hardware Requirements

| Component | Quantity | Purpose |
|---|---:|---|
| Arduino Uno | 1 | Main controller |
| HC-SR04 ultrasonic sensor | 1 | Measures distance to objects |
| Servo motor (e.g., SG90) | 1 | Rotates the sensor |
| Jumper wires | As required | Electrical connections |
| Breadboard | 1 | Prototyping and wiring |
| USB cable / suitable power supply | 1 | Powers and programs the Arduino |

## 💻 Software Requirements

- Arduino IDE
- Arduino-compatible C/C++ code
- Servo library, typically included with the Arduino IDE

## ⚙️ How It Works

The system follows a simple scanning process:

1. The Arduino commands the servo motor to move the ultrasonic sensor to a particular angle.
2. The ultrasonic sensor emits an ultrasonic pulse.
3. The sensor measures the time taken for the reflected echo to return.
4. The Arduino calculates the approximate distance to the detected object.
5. The angle and distance readings can be displayed or visualized.
6. The servo moves to another angle, and the process repeats.

### System Architecture

```text
        ┌──────────────────┐
        │   Arduino Uno    │
        └────────┬─────────┘
                 │
        ┌────────┴─────────┐
        │                  │
        ▼                  ▼
┌──────────────┐   ┌──────────────┐
│ Ultrasonic   │   │ Servo Motor  │
│ Sensor       │   │              │
└──────┬───────┘   └──────────────┘
       │
       ▼
 Distance Measurement
       │
       ▼
 Object Detection
```

*The diagram illustrates the main components conceptually. The Arduino controls both the sensor measurements and servo movement.*

## 🔌 Circuit Connections

Use the following as a reference if your build uses an HC-SR04 and an SG90 servo. Verify these against your actual wiring before publishing.

### HC-SR04 Ultrasonic Sensor

| Sensor Pin | Arduino Uno |
|---|---|
| VCC | 5V |
| GND | GND |
| TRIG | Digital pin 10 |
| ECHO | Digital pin 11 |

### Servo Motor

| Servo Wire | Connection |
|---|---|
| Signal | Digital pin 9 |
| VCC | Suitable 5V supply |
| GND | Common GND with Arduino |

**Power note:** Make sure the supply can provide sufficient current for the servo. If using an external supply, connect its ground to the Arduino ground. Avoid powering a servo from the Arduino's 5V pin if the current demand exceeds what the board and supply can safely provide.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Suyash282611/Radar_System.git
```

### 2. Open the project

Open the Arduino sketch (`.ino` file) in the Arduino IDE.

### 3. Connect the hardware

Wire the Arduino, ultrasonic sensor, and servo motor according to your circuit diagram.

### 4. Upload the code

- Select **Arduino Uno** under Tools → Board.
- Select the correct port under Tools → Port.
- Upload the sketch to the Arduino.

### 5. Test the system

Place an object in front of the sensor and observe the distance readings as the servo scans different angles.

*If your version includes a graphical interface, add the additional setup and execution instructions here.*

## 📷 Project Gallery

Add photographs of your actual hardware to the repository and display them here.

```text
images/
├── radar-system.jpg
├── circuit-connections.jpg
└── hardware-setup.jpg
```

```markdown
![Arduino Ultrasonic Radar System](images/radar-system.jpg)
```

## 🧠 What I Learned

Through this project, I explored:

- Interfacing an ultrasonic sensor with Arduino.
- Controlling a servo motor through code.
- Measuring distance using ultrasonic echo timing.
- Working with digital input and output pins.
- Combining multiple hardware components into one system.
- Understanding the fundamentals of embedded programming and object detection.

## 🔧 Challenges and Improvements

Potential areas to explore in future versions include:

- [ ] Displaying scan results on a computer using a graphical interface.
- [ ] Visualizing detected objects using angle and distance data.
- [ ] Improving measurement stability through filtering.
- [ ] Adding a buzzer or LED to indicate nearby objects.
- [ ] Designing a cleaner circuit layout or custom PCB.
- [ ] Improving the mechanical mounting of the sensor and servo.

## 📂 Project Structure

```text
Radar_System/
├── Radar_System.ino
├── README.md
└── images/
    ├── radar-system.jpg
    └── circuit-connections.jpg
```

## 🎯 Project Objective

The objective was to gain hands-on experience with Arduino, ultrasonic sensing, servo motor control, and basic object detection while developing a foundation for more advanced embedded systems and robotics projects.

## 👨‍💻 Author

**Suyash**

Electronics and Communication Engineering Student

- GitHub: [@Suyash282611](https://github.com/Suyash282611)
- LinkedIn: 

---

⭐ If you find this project useful, feel free to explore the code and build your own version.

