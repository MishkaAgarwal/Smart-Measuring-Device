# Smart Measuring Device

## Aim

To measure the distance between the device and an object and display the measurement on an OLED screen.

## What is the project?

A digital distance-measuring device that uses an ultrasonic sensor to estimate distance without physically touching an object.

## How does it work?

- The ultrasonic sensor emits a sound pulse above the range of human hearing.
- The pulse reflects off an object and returns to the sensor.
- The ESP32 measures the round-trip travel time.
- Distance is calculated as speed of sound multiplied by travel time, divided by two.
- The calculated distance is displayed on the OLED screen, in inches, feet and centimeters.
- The laser light can act as a visual pointer for the measuring direction, depending on its placement.
- The push button can freeze the measurement on the screen, so that it can be looked at.

## Components used

- ESP32 microcontroller
- Ultrasonic sensor
- OLED display
- Laser light module
- Breadboard
- Jumper wires
- Push Button

## Connections

| Component / Pin | Typical connection |
|---|---|
| ESP32 5V | Breadboard positive |
| ESP32 GND | Breadboard negative |
| Ultrasonic VCC | Breadboard positive |
| Ultrasonic GND | Breadboard negative |
| Ultrasonic TRIG | Pin 5 (ESP) |
| Ultrasonic ECHO | Pin 18 (ESP) |
| OLED VCC | Breadboard positive |
| OLED GND | Breadboard negative |
| OLED SDA | Pin 21 (ESP) |
| OLED SCL/SCK | Pin 22 (ESP) |
| Laser module S | Pin 15 (ESP) |
| Laser module + | Breadboard positive |
| Laser module - | Breadboard negative |
| Push Button | Pin 4 (ESP) |
| Push Button | Breadboard negative |
