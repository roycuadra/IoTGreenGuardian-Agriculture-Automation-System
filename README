# IoT Based Smart Agriculture & Automatic Irrigation System

Adafruit GFX Library: [Download](https://github.com/adafruit/Adafruit-GFX-Library)
SSD1306 Library: [Download](https://github.com/adafruit/Adafruit_SSD1306)   

# Circuit Diagram & Connection
Let us see the schematic of the IoT Smart Agriculture & Automatic Irrigation System project. I use Fritzing to make an schematic for most of my projects. All you need is to place and connect a component that is super easy.
![alt text](IoT-Smart-Agriculture-Automatic-Irrigation-System-640x300.jpg)
Connect the soil moisture sensor to A0 of Nodemcu and DHT11 to D4 Pin. The motor connects to Relay. To control the relay, we use the D5 Pin of NodeMCU. Connect the OLED display to the I2C pin of NodeMCU. You can power the Motor and Relay using the 5V pin of NodeMCU. The DHT11 Sensor, Capacitive Soil Moisture Sensor, and OLED Display require a 3.3V Supply only.
![alt text](4.jpg)

# Setting Up Thingspeak Server
Now we need to setup the Thingspeak Account. To set up Thingspeak follow the following Steps:

## Step 1: Visit https://thingspeak.com/ and create your account by filling up the details.
![alt text](./1.jpg)

## Step 2: Create a New Channel by Clicking on “Channel” & fill up the following details as shown in the image below.


Step 3: Click on API Key, you will see the “Write API Key“. Copy the API Key. This is very important, it will be required in Code Part.


Step 4: You can click on the “Private View” & customize the display window as you want.



The most important part of this code is the calibration of the Soil Moisture Sensor Value like AirValue and WaterValue. To learn how to calibrate and get the correct reading follow this post: Calibrating Soil Moisture Sensor Value. Please!, do not skip this step. This may result in getting the wrong soil moisture value and sometimes may result in continuous turning ON of the motor.