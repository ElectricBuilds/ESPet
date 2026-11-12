# 🐾 ESP32 PET

### A DIY Virtual Pet Powered by ESP32

**ESP32 PET** is an embedded virtual companion project designed to bring a digital pet to life using an ESP32 microcontroller. Built around a compact OLED display, the project aims to combine interactive gameplay, animated expressions, sound effects, and real-time battery monitoring into a small portable device.

The project takes inspiration from classic virtual pet systems while exploring embedded programming, human-machine interaction, and low-power electronics.

---

## 🌟 Project Overview

ESP32 PET is designed to behave like a small digital companion with its own needs, emotions, and personality.

The user will be able to interact with the pet through capacitive touch inputs, monitor its condition, and experience different animations and reactions through the OLED interface.

The firmware is being developed with a focus on lightweight execution, responsive interaction, and efficient resource usage.

## ✨ Planned Features

- 🐾 **Virtual Companion** — An animated digital pet with different expressions and emotional states.
- 😊 **Emotion System** — Happiness and mood that change based on user interaction.
- 🍎 **Feeding System** — Feed the pet to maintain its hunger level.
- 🎮 **Interaction System** — Interact with the pet using capacitive touch controls.
- ⚡ **Energy System** — Manage the pet's energy and activity.
- 😴 **Sleep Mode** — Allow the pet to rest and recover.
- ❤️ **Health System** — Track the pet's overall condition.
- 🔊 **Sound Effects** — Buzzer-generated audio feedback and notifications.
- 🔋 **Battery Monitoring** — Monitor battery voltage through an analog voltage sensor.
- 🖥️ **OLED Interface** — A custom monochrome graphical interface.

*Features will be implemented progressively as development continues.*

---

## 🛠️ Hardware Requirements

| Component | Specification |
|---|---|
| Microcontroller | ESP32 DevKitC |
| Display | 0.96-inch SSD1306 OLED |
| Display Resolution | 128 × 64 |
| Battery | 3.7V 18650 Li-ion |
| Charging Module | TP4056 |
| Audio | Piezo Buzzer |
| Voltage Monitoring | 0–25V Voltage Sensor |
| Interaction | 2 Touch GPIOs |

## 🔌 GPIO Pin Configuration

| Component | ESP32 GPIO |
|---|---|
| OLED SDA | GPIO 21 |
| OLED SCL | GPIO 22 |
| Buzzer | GPIO 25 |
| Voltage Sensor Output | GPIO 34 |
| Feed Touch | GPIO 27 |
| Play Touch | GPIO 32 |
| Sleep Touch | GPIO 33 |

All GPIO assignments are subject to change during hardware development.

## 🖥️ Display Interface

The project uses a 128×64 SSD1306 monochrome OLED display.

The planned interface includes:

| Screen | Purpose |
|---|---|
| Home | Main pet animation and expressions |
| Food | Feeding interaction |
| Play | Pet entertainment |
| Sleep | Rest and energy recovery |
| Statistics | Hunger, happiness, energy and health |
| Battery | Battery voltage and estimated charge level |

The interface will prioritize simple navigation, readable graphics, and lightweight animations.

## 🔋 Power Management

ESP32 PET is designed around a rechargeable 18650 lithium-ion battery.

The planned power architecture includes:

- 18650 rechargeable battery.
- TP4056 charging module.
- Battery protection.
- Regulated power supply for the ESP32.
- Analog battery voltage monitoring.

**Power safety:** The battery must not be connected directly to the ESP32 3.3V or 5V pins. An appropriate regulated supply and compatible battery protection circuit are required. The voltage sensor output must remain within the ESP32 ADC input limits.

## 💻 Software & Development

### Development Environment

- Arduino IDE
- Arduino ESP32 Core

### Planned Libraries

- Adafruit SSD1306
- Adafruit GFX Library

### Programming Language

C / C++ (Arduino Framework)

## 📂 Project Structure

The intended repository structure is:

```text
ESP32-PET/
│
├── README.md
├── LICENSE
├── ESP32-PET.ino
│
├── src/
│   ├── display.cpp
│   ├── pet.cpp
│   ├── interaction.cpp
│   ├── audio.cpp
│   └── battery.cpp
│
├── include/
│   └── config.h
│
├── assets/
│   └── sprites/
│
└── docs/
    └── wiring.md
```

The structure may evolve as the firmware becomes more modular.

## 🚧 Development Roadmap

### Phase 1 — Hardware Foundation
- [ ] Assemble ESP32 and OLED.
- [ ] Initialize SSD1306 display.
- [ ] Test buzzer output.
- [ ] Configure capacitive touch inputs.
- [ ] Implement battery voltage measurement.
- [ ] Establish stable battery-powered operation.

### Phase 2 — Virtual Pet Engine
- [ ] Design the main pet character.
- [ ] Implement facial expressions.
- [ ] Create animation sequences.
- [ ] Develop the hunger system.
- [ ] Develop happiness and energy statistics.
- [ ] Implement health mechanics.

### Phase 3 — Interaction
- [ ] Implement feeding.
- [ ] Implement play interactions.
- [ ] Implement sleep and recovery.
- [ ] Add sound effects.
- [ ] Implement screen navigation.

### Phase 4 — Advanced Features
- [ ] Persistent pet statistics.
- [ ] Improved animation system.
- [ ] Battery status interface.
- [ ] Power optimization.
- [ ] Final enclosure design.

## 🎯 Project Goals

ESP32 PET aims to demonstrate how a relatively small microcontroller can power an interactive digital companion.

Beyond creating a virtual pet, the project explores:

- Embedded systems programming.
- OLED graphics and animation.
- Capacitive touch sensing.
- Analog voltage measurement.
- Battery-powered electronics.
- Modular firmware architecture.

## 📜 License

ESP32 PET is licensed under the **Mozilla Public License 2.0 (MPL-2.0)**.

You may use, modify, and distribute this project's source code under the terms of the license.

Modifications to MPL-covered files must remain available under the MPL when distributed, subject to its terms.

See the [LICENSE](LICENSE) file for the complete license text.

Official license: https://www.mozilla.org/MPL/2.0/

---

## 🐾 ESP32 PET
@ ESPet is a Registered Trademark Of ElectricBuilds @
