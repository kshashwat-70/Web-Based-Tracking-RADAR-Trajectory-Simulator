# 📡 Web-Based Tracking RADAR Trajectory Simulator

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Java](https://img.shields.io/badge/Java-17%2B-orange)](https://www.oracle.com/java/technologies/javase-downloads.html)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-blue)](#)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-brightgreen)](#contributing)

A powerful, real-time, web-based simulator designed to track RADAR trajectories by converting and visualizing spatial coordinates. Built in Java and enhanced with HTML/JavaScript for dynamic data visualization, this tool allows seamless transformation and transmission of ECEF, ENV, or LLA data for simulation and analysis.

---

## 📚 Table of Contents

- [🚀 Features](#-features)
- [🏗️ Architecture](#-architecture)
- [🛠️ Installation](#-installation)
- [📊 Usage](#-usage)
  - [📡 Launch the Sender Module](#-launch-the-sender-module)
  - [📶 Start the Receiver Module](#-start-the-receiver-module)
  - [📊 Visualize the Data](#-visualize-the-data)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)
- [🙌 Acknowledgements](#-acknowledgements)

---

## 🚀 Features

✅ **Real-Time Simulation**: View RADAR parameters in real-time with continuous updates.  
✅ **Flexible Coordinate Support**: Converts Earth-Centered Earth-Fixed (ECEF), East-North-Vertical (ENV), or Latitude-Longitude-Altitude (LLA) coordinates into RADAR-friendly format.  
✅ **Multi-Axis Visualization**: Simultaneous graphing of Azimuth Angle, Elevation Angle, and Range on an intuitive interface.  
✅ **High-Performance Networking**: Efficient data transmission from sender to receiver module using Java sockets and multithreading.  
✅ **Web-Based Display**: Output visualizations rendered via HTML5 and JavaScript.

---

## 🏗️ Architecture

This simulator is divided into two core modules:

### 📨 Sender Module

- **Function**: Reads spatial coordinate data, converts it to RADAR parameters (range, theta, phi), and transmits the results over the network.
- **Tech Stack**: Java (JDK 17+), multithreading, socket programming.

### 📥 Receiver Module

- **Function**: Listens for incoming data from the sender, processes the stream, and passes the information to a browser-based visualizer.
- **Tech Stack**: Java for backend + HTML/CSS/JavaScript for frontend visualization.

---

## 🛠️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/kshashwat-70/Web-Based-Tracking-RADAR-Trajectory-Simulator.git
cd Web-Based-Tracking-RADAR-Trajectory-Simulator
 ```
2. **Set Up the Development Environment:**

- Ensure [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) is installed.
- Use an IDE like [IntelliJ IDEA](https://www.jetbrains.com/idea/) or [Eclipse](https://www.eclipse.org/).

3. **Compile the Java Files:**

```bash
javac SenderModule.java ReceiverModule.java
```

4. **Prepare the Web Interface:**

Open `RadarSimulator.html` in a web browser to visualize the RADAR parameters.

---

## 📊 Usage

### 📡 Launch the Sender Module

1. Execute `SenderModule.java`.

```bash
java SenderModule
```

2. Input the path to your coordinate dataset (ECEF, ENV, or LLA).

The module will process and transmit the data.

### 📶 Start the Receiver Module

1. Run `ReceiverModule.java`.

```bash
java ReceiverModule
```

The receiver will collect incoming RADAR data and pass it to the visualization module.

### 📊 Visualize the Data

1. Open the `RadarSimulator.html` file in a compatible web browser.

2. Observe the dynamic graphs displaying:

- **Azimuth Angle**
- **Elevation Angle**
- **Range**

---

## 🤝 Contributing

Contributions are welcome! Here’s how you can get involved:

1. **Fork the Repository:**

2. **Create a New Branch:**

```bash
git checkout -b feature/your-feature
```

3. **Make Your Changes and Commit:**

```bash
git commit -m "Add your feature"
```

4. **Push to Your Branch:**

```bash
git push origin feature/your-feature
```

5. **Submit a Pull Request.**

---



---

## 🙌 Acknowledgements

- **ECEF Coordinate System**: [Earth-Centered, Earth-Fixed Reference](https://en.wikipedia.org/wiki/ECEF)
- **Java Networking**: [Java Networking Tutorial](https://docs.oracle.com/javase/tutorial/networking/)

For issues or questions, please open an [issue](https://github.com/mitul-goswami/Web---Based-Tracking-RADAR-Trajectory-Simulator/issues).

---

⭐ **If you find this project helpful, please consider giving it a star!**

