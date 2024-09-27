# ESP32-CAM Video Streaming Project

Welcome to the ESP32-CAM Video Streaming Project! This repository contains everything you need to set up your **ESP32-CAM** module to stream video over **Wi-Fi**. With just a few components, you can turn your ESP32-CAM into a powerful video streaming device.

## Requirements

To get started, you'll need the following components:

- **One ESP32-CAM (Ai Thinker)**
- **One USB to TTL Converter or FTDI Module**
- **Female-to-female jumper wires**

## Wiring Configuration

To connect your `ESP32-CAM` to the `USB to TTL` converter or `FTDI` module, follow the wiring configuration below:

| ESP32-CAM       | USB to TTL or FTDI Programmer |
|------------------|------------------------------|
| GND              | GND                          |
| 5V               | VCC (5V)                    |
| U0R              | TX                           |
| U0T              | RX                           |
| GPIO 0          | GND                          |

### Important Notes

- **GPIO 0** must be connected to **GND** to upload a sketch.
- After connecting **GPIO 0 to GND**, press the ESP32-CAM on-board **RESET** button to put your board in flashing mode.

## Getting Started

1. **Clone this repository:**

   ```bash
   git clone https://github.com/yourusername/esp32-cam-video-streaming.git
   cd esp32-cam-video-streaming


2.  **Install the required libraries:**
    
    Make sure you have the necessary libraries installed in your Arduino IDE. 
    Add this URL in File > Preference > Additional Board Manager :
    ```bash
    https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json   
    
3.  **Upload the sketch:**
    
    Open the provided Arduino sketch in the Arduino IDE, select the appropriate board and port, and upload it.
    
4.  **Connect to the ESP32-CAM Wi-Fi:**
    
    Once the upload is complete, disconnect `GPIO 0` from `GND `and `reset` the **ESP32-CAM**. It will start broadcasting a Wi-Fi signal. Connect to it using your smartphone or computer.
    
5.  **Access the video stream:**
    
    Open a web browser and enter the IP address provided in the serial monitor to view the video stream.
     you can see the local IP in **Serial Monitor**.
     ```python
     #Default Local IP Address
     192.168.4.1    
---
```python

Feel free to modify any sections as needed!
#Pezhvak ;)
