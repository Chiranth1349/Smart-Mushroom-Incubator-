# Smart Mushroom Incubator

Smart IoT-based incubator built for the Social Hackathon 2025, designed to monitor and control mushroom growth environments for urban and small-scale farming.

## Features

- Automatic and Manual control modes
- Real-time control via mobile app and physical controller
- Adjustable temperature, humidity, water spray, and airflow
- Auto profiles for Oyster, Button, and Shiitake mushrooms
- Built with ESP32, DHT22, CPU fans, mist nozzles, diaphragm pump, and LCD display

## Components Used

- **Microcontroller**: ESP32-WROOM-32
- **Sensor**: DHT22 (temperature & humidity)
- **Actuators**: 
  - CPU fans for airflow
  - Diaphragm pump + mist nozzle for humidity
- **Relay Modules**: 2-channel for fans and spray
- **Display**: I2C LCD 16x2
- **Interface**: 
  - 3 Buttons: Mode, Set, Start
  - Potentiometer for selection
- **Power**: SMPS
- **App**: MIT App Inventor-based mobile control

## Modes

### Manual Mode
- Set temperature (30–70°C)
- Set humidity
- Fan and spray durations
- Total operation time

### Auto Mode
- Choose mushroom type: Oyster, Button, or Shiitake
- Automatically applies optimal settings

## Known Issues
- ESP32 became unstable during the final presentation; may require firmware cleanup or hardware debouncing.
- Sending Data from ESP32 was Hard and unstable to the MIT app, compared to Receiving Data on the ESP32 from the MIT App Inventor 

## Author

A M Chiranth 

## License

MIT License
