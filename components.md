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
