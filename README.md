# IoT Agent
<!-- NodeMCU IoT Project with MiA IoT Platform -->

This project demonstrates the use of a NodeMCU board to interact with the [**MiA (Middleware in Action)**](https://github.com/I1820/mia) IoT platform. The NodeMCU collects sensor data and sends it to the MiA broker using the MQTT protocol. The platform allows users to control and monitor IoT devices in real-time.

## Features

- Connects NodeMCU to MiA, the IoT platform
- Uses MQTT protocol for communication
- Sends sensor data (e.g., light intensity) to the broker

## Installation

This section explains how to run an IoT agent. For instructions about running the MiA server, refer to [this guide](https://github.com/I1820/mia).

1. **Clone the Repository:**
   ```
   git clone <repository-link>
   ```

2. **Open the Project:**
   - If using Arduino IDE: Open `src/main.cpp`.
   - If using PlatformIO: Open the project folder in your preferred code editor.

3. **Install Dependencies:**
   Install the required libraries using the Arduino Library Manager or PlatformIO.

   - PubSubClient for MQTT communication
   - WiFi for connecting to your network

4. **Configure Wi-Fi and MiA Broker:**
   Add the `src/arduino_secrets.h` file to set your Wi-Fi credentials and the MiA broker details:

   ```c
    #define SECRET_SSID "your_SSID"
    #define SECRET_PASS "your_password"
    #define BROKER_IP "MiA_server_address"
   ```

5. **Upload to NodeMCU:**
   Connect your NodeMCU to your computer and upload the code using the appropriate method (Arduino IDE or PlatformIO).
