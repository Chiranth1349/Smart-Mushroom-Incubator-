# Smart Mushroom Incubator

Smart IoT-based mushroom incubator developed for **Social Hackathon 2025** and **Yukthi 2025**, designed to monitor and control critical environmental parameters required for efficient mushroom cultivation.  
The system is aimed at urban and small-scale farming with a focus on reliability, automation, and remote monitoring.

---

## Features

- Manual control using physical switches
- Real-time monitoring of environmental parameters
- Temperature and humidity sensing
- CO₂ level monitoring (trend-based)
- Water level monitoring
- Light brightness sensing
- Automated pump scheduling
- Local system status display using LCD
- Remote monitoring and control via MQTT
- Wi-Fi enabled using ESP32

---

## Components Used

### Sensors
- **DHT22** → Temperature & Humidity  
- **MQ135** → CO₂ sensing (Analog input)  
- **Water Level Sensor** → Analog input (GPIO 35)  
- **LDR (Light Dependent Resistor)** → Light brightness sensing (GPIO 33)

### Actuators (Relays)
- **Fan Relay** → GPIO 5  
- **Light Relay** → GPIO 18  
- **Pump Relay** → GPIO 19  

### Switches (Manual Override)
- **Fan Switch** → GPIO 14  
- **Light Switch** → GPIO 27  
- **Pump Switch** → GPIO 26  

### Display
- **20×4 I2C LCD Display** (I2C Address: `0x27`)

### Microcontroller
- **ESP32-WROOM-32**

### Connectivity
- **Wi-Fi** (ESP32 built-in)  
- **MQTT** (HiveMQ Cloud)

---

## Operating Modes

### Manual Mode
- Fan, light, and pump can be toggled using physical switches
- Live system parameters displayed on LCD
- Pump runs on scheduled automation unless manually overridden

### Cloud Control (MQTT)
- Remote relay control
- Emergency stop (E-STOP) functionality
- Telemetry data transmission including:
  - Temperature
  - Humidity
  - CO₂ level
  - Water level
  - Brightness
  - Relay states

---

## Hardware Version

- **Version:** v2  
- Improved enclosure and layout
- Integrated control box
- Expanded sensor set
- Stable relay control and pump scheduling logic

---

## Known Issues

- CO₂ readings are **trend-based** and not laboratory calibrated
- DHT22 may return invalid values if power or wiring is unstable
- MQTT reliability depends on network connectivity

---

## Author

**A M Chiranth**

---

## License

**MIT License**