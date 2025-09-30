# IOT-BASED-WEATHER-MONITORING-SYSTEM-WITH-WIFI-AND-FAN-MODULE-
 
# ❄️ Smart Temperature Monitoring and Fan Control System
# Project Overview
This project implements a Smart IoT Temperature Monitoring and Fan Control System using an ESP32 microcontroller, a DHT22 temperature/humidity sensor, and an I2C LCD display. The system monitors ambient temperature, automatically controls a cooling fan based on a set threshold, and reports all data to the ThingSpeak cloud platform for real-time visualization and remote tracking.
This solution is perfect for managing the climate in small rooms, server closets, or greenhouses, ensuring the temperature remains within an acceptable range and providing an alert for high-temperature conditions.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# ⚙️ Key Features
# .Real-time Temperature & Humidity Monitoring:
Uses the DHT22 sensor for accurate readings.
# .Automatic Fan Control: 
The system automatically switches a fan (simulated by a digital pin/LED) ON when the temperature exceeds 50 ∘C and OFF when it drops below this threshold.
# .High-Temperature Alert: 
Triggers an "ALERT!" message on the LCD and activates a visual indicator (simulated by a digital pin/LED) when the temperature exceeds the threshold.
# .Cloud Integration (ThingSpeak):
Sends temperature, fan status, and alert status to a ThingSpeak channel for data logging and graphical visualization.
# .Local Display:
An I2C LCD provides immediate feedback on the current temperature, fan status, and alert condition.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 🧱 Hardware Components
| **Component**        | **Description**                                                                             |
| -------------------- | ------------------------------------------------------------------------------------------- |
| **ESP32**            | A powerful microcontroller with built-in Wi-Fi capability, used for controlling the system. |
| **DHT22**            | A temperature and humidity sensor used to monitor the environment.                          |
| **16x2 LCD Display** | A Liquid Crystal Display (LCD) to show the temperature and humidity readings.               |
| **Red LED**          | A visual indicator to show when the temperature is above a certain threshold (fan ON).      |
| **Green LED**        | A visual indicator to show when the temperature is within the acceptable range (fan OFF).   |
| **Resistors**        | Used with the LEDs to limit current and prevent damage.                                     |
| **Jumper Wires**     | Wires used for connecting components on the breadboard.                                     |
| **Breadboard**       | A platform for connecting all the components together without soldering.                    |


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 🔌 Circuit Diagram and Wiring
Component Pin	ESP32 Pin	Purpose

DHT22 Data	GPIO 4	Temperature/Humidity Data Input

I2C LCD SDA	GPIO 21	I2C Data Line

I2C LCD SCL	GPIO 22	I2C Clock Line

Red LED Anode	GPIO 16	High-Temperature Alert Indicator

Green LED Anode	GPIO 17	Fan Status Indicator
