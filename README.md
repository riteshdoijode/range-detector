# Arduino Motion Detector with PIR Sensor and LED Alert

This project is a simple motion detector built using an Arduino board, a PIR motion sensor, and an LED. When motion is detected, the LED lights up for a short duration.

## 🚀 Features

- Detects motion using a PIR (Passive Infrared) sensor.
- Lights up an LED when movement is detected.
- Adjustable delay and easy to customize.

## 🛠️ Components Used

- Arduino Uno (or compatible board)
- PIR Motion Sensor (HC-SR501)
- LED
- 220Ω resistor
- Jumper wires
- Breadboard

## 🧠 How It Works

The PIR sensor detects motion in its field of view. When it senses movement, it sends a HIGH signal to the Arduino. The Arduino then turns on the LED for 3 seconds.

## 💾 Code

The main logic is in `sketch_aug11a.ino`.

```cpp
if (digitalRead(sensor) == HIGH) {
    digitalWrite(led, HIGH);
    delay(3000);
    digitalWrite(led, LOW);
}
```

## 🔧 Setup

1. Connect the PIR sensor:
   - VCC → 5V
   - GND → GND
   - OUT → Digital Pin 2

2. Connect the LED:
   - Positive (long leg) → Digital Pin 13 (through 220Ω resistor)
   - Negative (short leg) → GND

3. Sketch to your Arduino.

![1506106762614](https://github.com/user-attachments/assets/43965d83-6f34-497a-8880-8ddd0c864301)

## 📄 License

This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for more details.

## 🤝 Contributions

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.
