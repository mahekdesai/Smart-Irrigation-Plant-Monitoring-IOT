# Smart Plant Monitoring System with Blynk

Welcome to the Smart Plant Monitoring System repository! This project utilizes an ESP8266 microcontroller, a DHT11 sensor for temperature and humidity, and a soil moisture sensor. It communicates with the Blynk platform to monitor plant conditions and control a light indicator based on soil moisture levels. The following information will guide you through the project details and code.

## Code Overview

- **File:** `Smart_Plant_Monitoring.ino`

  This Arduino sketch reads temperature and humidity values from the DHT11 sensor, soil moisture from the analog sensor, and controls a light indicator. It communicates with the Blynk app for real-time monitoring and notifications.

## Hardware Components

1. **ESP8266 Microcontroller**
2. **DHT11 Sensor**
3. **Soil Moisture Sensor**
4. **LED (Light Indicator)**
5. **Resistors**
6. **Jumpers and Breadboard**

## Configuration

- **Blynk Setup:**
  - Replace `auth` with your Blynk authentication token.
  - Replace `ssid` and `pass` with your WiFi network credentials.

## Pin Configuration

- **DHT11 Sensor:**
  - `DHTPIN` - Data pin connected to D1.

- **Soil Moisture Sensor:**
  - `A0` - Analog pin connected to the sensor.

- **LED (Light Indicator):**
  - `Light` - Control pin connected to D2.

## Usage

1. **Blynk App:**
   - Create a Blynk account and set up a new project.
   - Add three Value Display widgets (V1 for humidity, V2 for temperature, V3 for soil moisture) and a Notification widget.

2. **Hardware Setup:**
   - Connect the hardware components based on the provided pin configuration.
   - Upload the code to your ESP8266 using the Arduino IDE.

3. **Monitor:**
   - Open the Blynk app to monitor real-time temperature, humidity, and soil moisture.
   - The LED light indicates the soil moisture status (on when moisture is low, off when moisture is sufficient).

4. **Notifications:**
   - Receive Blynk notifications when soil moisture levels drop below or rise above set thresholds.

## Additional Information

- Temperature and humidity values are read from the DHT11 sensor and displayed on the Blynk app.
- The soil moisture sensor determines soil moisture levels, and the LED light provides a visual indication.
- Notifications are sent to alert users when soil moisture conditions require attention.

## Contributions

Feel free to contribute to the project by improving the code, enhancing functionality, or adding features. Create a pull request with your changes.

If you encounter issues or have questions, please open an issue on GitHub.

Happy plant monitoring! 🌱📊
