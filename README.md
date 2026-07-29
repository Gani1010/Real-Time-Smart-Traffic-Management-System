# 🚦 Real-Time Smart Traffic Management System Using AI

An intelligent traffic management system that dynamically controls traffic signals based on real-time vehicle detection using **YOLOv8**, **Raspberry Pi**, and **Computer Vision**. Unlike traditional traffic lights with fixed timings, this system adjusts signal durations according to traffic density, helping reduce congestion and improve traffic flow.

---

## 📖 Project Overview

Traffic congestion is one of the biggest challenges in urban areas. Conventional traffic signals operate on fixed timers regardless of the number of vehicles waiting at an intersection, leading to unnecessary delays and increased fuel consumption.

This project uses Artificial Intelligence to detect and count vehicles in real time through a Raspberry Pi camera. Based on the detected traffic density, the system automatically adjusts the green signal duration for each lane. It also includes emergency vehicle detection to provide priority access when required.

---

## ✨ Features

* 🚗 Real-time vehicle detection using YOLOv8
* 📹 Live video processing with Raspberry Pi Camera
* 🔄 Servo motor rotates the camera to monitor multiple lanes
* 🚦 Automatic traffic signal control
* ⏱️ Dynamic signal timing based on vehicle count
* 🚑 Emergency vehicle detection with signal priority
* 📊 Live countdown timer using TM1637 4-digit display
* ⚡ Raspberry Pi GPIO control for LEDs and hardware components
* 🧠 AI-powered traffic optimisation

---

## 🛠 Hardware Components

* Raspberry Pi 4 Model B (4 GB)
* Raspberry Pi Camera Module
* SG90 / MG996R Servo Motor
* TM1637 4-Digit Display
* Red, Yellow and Green LEDs
* Breadboard
* Jumper Wires
* Power Supply

---

## 💻 Software & Technologies

* Python
* YOLOv8 (Ultralytics)
* OpenCV
* PyTorch
* Raspberry Pi OS
* GPIOZero
* RPi.GPIO
* Label Studio (Dataset Annotation)

---

## 🏗 System Architecture

```text
Camera
   │
   ▼
YOLOv8 Vehicle Detection
   │
   ▼
Vehicle Counting
   │
   ▼
Traffic Decision Logic
   │
   ├── Green Signal Time Calculation
   ├── Emergency Vehicle Detection
   └── Lane Selection
          │
          ▼
Raspberry Pi GPIO
          │
          ├── Traffic LEDs
          ├── Servo Motor
          └── TM1637 Countdown Display
```

---

## 🚦 Traffic Signal Logic

| Vehicle Count              | Green Signal Time  |
| -------------------------- | ------------------ |
| 0 Vehicles                 | 5 Seconds          |
| 1–2 Vehicles               | 30 Seconds         |
| 4 or More Vehicles         | 40 Seconds         |
| Emergency Vehicle Detected | Immediate Priority |

---

## 📂 Project Structure

```text
Real-Time-Smart-Traffic-Management-System/
│
├── src/
│   ├── main.py
│   ├── object_detection.py
│   ├── traffic_controller.py
│   ├── servo_control.py
│   └── led_control.py
│
├── model/
│   └── best.pt
│
├── images/
│
├── videos/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## ⚙ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/Real-Time-Smart-Traffic-Management-System.git
```

Move into the project folder:

```bash
cd Real-Time-Smart-Traffic-Management-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python src/main.py
```

---

## 📸 Project Demonstration

Add screenshots of:

* Hardware setup
* Raspberry Pi connections
* Live vehicle detection
* Traffic signal operation
* Countdown timer
* Emergency vehicle detection

Example:

```
images/
├── setup.jpg
├── detection.png
├── traffic_signal.png
└── output.png
```

---

## 🎯 Applications

* Smart Cities
* Intelligent Transportation Systems
* Traffic Congestion Management
* Emergency Vehicle Routing
* Urban Traffic Monitoring
* AI-Based Infrastructure

---

## 🚀 Future Enhancements

* Multi-camera traffic monitoring
* Cloud-based dashboard
* Real-time analytics
* Number plate recognition (ANPR)
* Traffic prediction using Machine Learning
* Mobile application for live monitoring
* Integration with IoT platforms
* Smart city deployment

---

## 📈 Benefits

* Reduces traffic congestion
* Minimises waiting time
* Improves emergency response
* Optimises fuel consumption
* Reduces carbon emissions
* Enhances road safety
* Efficient traffic signal management

---

## 📚 Tech Stack

| Category             | Technologies       |
| -------------------- | ------------------ |
| Programming Language | Python             |
| AI Model             | YOLOv8             |
| Computer Vision      | OpenCV             |
| Deep Learning        | PyTorch            |
| Annotation Tool      | Label Studio       |
| Hardware             | Raspberry Pi 4     |
| Display              | TM1637             |
| Motor                | SG90 / MG996R      |
| GPIO Library         | RPi.GPIO, GPIOZero |

---

## 👨‍💻 Author

Gani1010
Electronics and Communication Engineering (ECE)

Passionate about Artificial Intelligence, Computer Vision, Embedded Systems, IoT and Software Development.

GitHub: https://github.com/Gani1010

---

## ⭐ Support

If you found this project useful, consider giving it a **⭐ Star** on GitHub. It helps others discover the project and motivates further improvements.

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
