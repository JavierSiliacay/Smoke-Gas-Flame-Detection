# Fire and Gas Detection System

This project demonstrates a fire and gas detection system using an Arduino. The system utilizes a flame sensor and an MQ2 gas sensor to detect hazardous conditions, activating different LEDs and a buzzer for alerts. It provides a simple, efficient way to monitor fire and gas risks.

## 🔧 Hardware Components

- Arduino Uno (or compatible board)
- 1 x Flame Sensor
- 1 x MQ2 Gas Sensor
- 1 x Red LED (for flame detection)
- 1 x Orange LED (for gas/smoke detection)
- 1 x Green LED (for normal condition)
- 1 x Buzzer (for alerts)
- Jumper wires
- Resistors

## 📋 Pin Configuration

| Component           | Arduino Pin |
|---------------------|-------------|
| Flame Sensor        | A0          |
| Gas Sensor          | A1          |
| Red LED (Flame)     | 5           |
| Orange LED (Gas)    | 6           |
| Green LED (Normal)  | 7           |
| Buzzer              | 2           |

## 🧠 Functionality

- **Flame Detection**: 
  - If the flame sensor detects a flame (value < 500), the **Red LED** lights up and a buzzer emits a 4kHz tone for 1 second.
  
- **Gas/Smoke Detection**:
  - If the gas sensor detects gas/smoke (value between 300 and 600), the **Orange LED** lights up and a buzzer emits a 3.5kHz tone for 0.5 seconds.

- **Normal Condition**: 
  - When no flame or gas is detected, the **Green LED** lights up indicating normal conditions.

## 🧾 How It Works

1. The system continuously reads the flame and gas sensors.
2. If a flame is detected, the red LED lights up, and an alert tone is emitted.
3. If gas or smoke is detected, the orange LED lights up, and a different alert tone is emitted.
4. If no hazard is detected, the green LED lights up to indicate normal conditions.

## 🛠️ Setup Instructions

1. Connect all components according to the pin configuration table above.
2. Upload the provided Arduino sketch to your Arduino board.
3. The system will continuously monitor for flame and gas conditions.
4. The LEDs and buzzer will respond based on the detected sensor values.

## 📝 License

This project is open-source and free to use under the MIT License.

---

Made with ❤️ by Javier Siliacay | USTP 🇵🇭
