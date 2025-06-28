# Air Quality Monitoring System using ESP8266, DHT11, and Blynk

This Arduino project monitors air quality using a gas sensor (MQ series), DHT11 temperature and humidity sensor, and displays data on an OLED screen. It also sends live data and alerts to the Blynk IoT platform.

## 📡 Features
- OLED display cycling temperature, humidity, air quality, and system status
- WiFi + Blynk integration to send real-time data
- Pollution alerts via Blynk Events
- Error handling for DHT11 and OLED
- Multi-page screen display with status indicators

## 🛠 Hardware Used
- NodeMCU (ESP8266)
- DHT11 Sensor
- MQ Gas Sensor
- 0.96” I2C OLED Display
- WiFi Network

## 🔌 Circuit Connections
| Component | ESP8266 Pin |
|----------|--------------|
| DHT11    | GPIO2 (D4)   |
| MQ Gas   | A0           |
| OLED SDA | D2 (GPIO4)   |
| OLED SCL | D1 (GPIO5)   |

## 🔧 Libraries Used
- `ESP8266WiFi.h`
- `BlynkSimpleEsp8266.h`
- `Adafruit_GFX.h`
- `Adafruit_SSD1306.h`
- `DHT.h`

## 🧠 How it works
1. Reads temperature, humidity, and gas values.
2. Displays them on the OLED screen in a page-wise manner.
3. Sends data to Blynk dashboard every 30 seconds.
4. Alerts if air quality exceeds the threshold.

## 💡 Customize
- Replace WiFi credentials and Blynk Auth Token.
- Adjust `sensorThreshold` if needed for your MQ sensor.

## 📸 Demo
(You can add a screenshot of your OLED display or Blynk dashboard here)

## 📄 License
MIT
