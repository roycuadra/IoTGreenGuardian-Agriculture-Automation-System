# Cloud IoT Smart Agriculture Automatic Irrigation System

This repository contains the code and documentation for building a Cloud IoT Smart Agriculture Automatic Irrigation System using NodeMCU, soil moisture sensor, DHT11 sensor, motor, relay, and an OLED display.

## Components Used

- NodeMCU
- Soil Moisture Sensor
- DHT11 Sensor
- Motor
- Relay
- OLED Display (SSD1306)

## Circuit Diagram & Connection

![Circuit Diagram](./images/Schematic%20Diagram.jpg)

1. Connect the soil moisture sensor to `A0` of NodeMCU.
2. Connect the DHT11 sensor to `D4` pin of NodeMCU.
3. Connect the motor to the relay.
4. Control the relay using `D5` pin of NodeMCU.
5. Connect the OLED display to the I2C pins of NodeMCU.
6. Power the Motor and Relay using the `5V` pin of NodeMCU.
7. The DHT11 Sensor, Capacitive Soil Moisture Sensor, and OLED Display require a `3.3V` supply.

## Setting Up ThingSpeak Server

Follow these steps to set up ThingSpeak for data visualization:

1. Create an account on [ThingSpeak](https://thingspeak.com/).
2. Create a new channel with the required fields.
   - Field 1: Soil Moisture
   - Field 2: Temperature
   - Field 3: Humidity
3. Click on API Keys and copy the "Write API Key".

## Code Configuration

1. Download the required libraries:
   - [Adafruit GFX Library](https://github.com/adafruit/Adafruit-GFX-Library)
   - [SSD1306 Library](https://github.com/adafruit/Adafruit_SSD1306)

2. Configure the following parameters in the code:
   - WiFi SSID and password
   - ThingSpeak Write API Key
   - Calibration values for Soil Moisture Sensor (AirValue and WaterValue)

## Calibration

Calibrate the Soil Moisture Sensor Value for accurate readings. Refer to [Calibrating Soil Moisture Sensor Value](#) for detailed instructions.

## Usage

1. Upload the code to NodeMCU using the Arduino IDE.
2. The system will read soil moisture, temperature, and humidity values.
3. Data will be sent to ThingSpeak for visualization.
4. Automatic irrigation control based on soil moisture can be implemented using the relay and motor.

## Important Note

Ensure proper calibration of the Soil Moisture Sensor to avoid incorrect readings and continuous motor operation.
