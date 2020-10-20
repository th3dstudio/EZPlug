**This version of Tasmota is specifically for the [TH3D EZPlug wifi outlet](https://www.th3dstudio.com/product/ezplug-open-source-wifi-smart-plug/) for 3D Printers.**

## Features

- Built on Tasmota 8.5.X
- Presetup for our EZPlug products
- Home Assistant discovery enabled by default
- Works with OctoPrint-Tasmota plugin for Octoprint
- EZPlug+ has Power monitoring pre-calibrated for US voltage
- Supports upgrading to standard Tasmota for those that want it

## Updating your EZPlug Firmware

1. Download the latest releases for your plug (EZPlug or EZPlug+). **You will need the normal BIN file and the minimal BIN file**
2. Flash the minimal BIN file from the GUI
3. Flash the normal BIN file from the GUI
4. Enjoy the updated firmware

## Using the EZPlug to "Vanilla" Tasmota

Our plug is compatible with regular Tasmota when setup with the correct template.

**Tasmota Templates:**


- **EZPlug:** `{"NAME":"EZPlug V1","GPIO":[0,0,0,17,0,0,0,0,0,56,21,0,0],"FLAG":0,"BASE":1}`
- **EZPlug+:** `{"NAME":"EZPlug V1","GPIO":[0,0,0,17,134,132,0,0,131,56,21,0,0],"FLAG":0,"BASE":1}`

**Converting the EZPlug from our Firmware to Tasmota:**

1. Download the latest tasmota-minimal.bin and flash it from the GUI
2. Download the latest tasmota.bin and flash it from the GUI
3. Reset the EZPlug configuration to clear out our config to prevent errors
4. Use it with standard Tasmota!

## Contribute to the Tasmota Project

You can contribute to Tasmota by
- providing Pull Requests (Features, Proof of Concepts, Language files or Fixes)
- testing new released features and report issues
- donating to acquire hardware for testing and implementing or out of gratitude
- contributing missing [documentation](https://tasmota.github.io/docs) for features and devices

[![donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://paypal.me/tasmota)

## Credits

People helping to keep the show on the road:
- David Lang providing initial issue resolution and code optimizations
- Heiko Krupp for his IRSend, HTU21, SI70xx and Wemo/Hue emulation drivers
- Wiktor Schmidt for Travis CI implementation
- Thom Dietrich for PlatformIO optimizations
- Marinus van den Broek for his EspEasy groundwork
- Pete Ba for more user friendly energy monitor calibration
- Lobradov providing compile optimization tips
- Flexiti for his initial timer implementation
- reloxx13 for his [TasmoAdmin](https://github.com/reloxx13/TasmoAdmin) management tool
- Joachim Banzhaf for his TSL2561 library and driver
- Gijs Noorlander for his MHZ19, SenseAir and updated PubSubClient drivers
- Erik Montnemery for his HomeAssistant Discovery concept and many code tuning tips
- Federico Leoni for continued HomeAssistant Discovery support
- Aidan Mountford for his HSB support
- Daniel Ztolnai for his Serial Bridge implementation
- Gerhard Mutz for multiple sensor & display drivers, Sunrise/Sunset, and scripting
- Nuno Ferreira for his HC-SR04 driver
- Adrian Scillato for his (security)fixes and implementing and maintaining KNX
- Gennaro Tortone for implementing and maintaining Eastron drivers
- Raymond Mouthaan for managing Wemos Wiki information
- Norbert Richter for his [decode-config.py](https://github.com/tasmota/decode-config) tool
- Andre Thomas for providing [thehackbox](http://thehackbox.org/tasmota/) OTA support and daily development builds
- Joel Stein, digiblur and Shantur Rathore for their Tuya research and driver
- Frogmore42 for providing many issue answers
- Jason2866 for platformio support and providing many issue answers
- Blakadder for managing the new document site and providing template management
- Stephan Hadinger for refactoring light driver, enhancing HueEmulation and Zigbee support
- tmo for designing the official Tasmota logo
- Stefan Bode for his Shutter and Deep sleep drivers
- Jacek Ziółkowski for his [TDM](https://github.com/jziolkowski/tdm) management tool and [Tasmotizer](https://github.com/tasmota/tasmotizer) flashing tool
- Christian Staars for NRF24L01 and HM-10 Bluetooth sensor support
- Paul Diem for UDP Group communication support
- Jörg Schüler-Maroldt for his initial ESP32 port
- Javier Arigita for his thermostat driver
- Many more providing Tips, Wips, Pocs, PRs and Donations

## License

This program is licensed under GPL-3.0
