# Oled-Bengali-Song-Player

An Arduino project that displays an introductory image followed by a 8-line loop of song lyrics frame-by-frame on a 128x64 I2C OLED display. However, I haven't included the bitmap array for the image in my code, you can add your own and adjust your array indexes in the loop.

## Features
* **Intro Image + Lyrics Loop:** Automatically displays an introductory title screen, then sequences through 8 lines of text continuously.
* **PROGMEM Storage:** Utilizes flash memory storage efficiently for smooth bitmap handling on microcontrollers.
* **Customizable Timings:** Easily adjustable delay times for individual slides/frames.

## Hardware Requirements
* Arduino-compatible board (e.g., Uno, Nano, ESP32)
* 128x64 I2C SSD1306 OLED Display

## Dependencies
Make sure you have the following Arduino libraries installed via the Library Manager:
* `Adafruit GFX Library`
* `Adafruit SSD1306`

## Wiring Guide
| OLED Pin | Arduino Pin |
| :--- | :--- |
| GND | GND |
| VCC | 5V or 3.3V |
| SCL | A5 (or SCL on ESP32) |
| SDA | A4 (or SDA on ESP32) |

## Usage
1. Open the `.ino` file in the Arduino IDE.
2. Replace the placeholder hex arrays with your generated 128x64 bitmap data (1 intro image + 8 lyrics frames).
3. Select your Board and COM port, then upload the sketch!