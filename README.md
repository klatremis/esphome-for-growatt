# ESPhome for Growatt by Klatremis (still under development)
ESPhome configuration for monitoring and control of Growatt inverters in Home Assistant.
This include all addresses i could see relevant from the inverter.

* For DIY generic esp32 hardware, use "esp32" and the wiring below
* For KlatremisHW, use "klatremishw" code

## Supported devices
### SPH inverters
* SPH3600 (confirmed)
* SPH10000TL3 (not confirmed)

### MIC inverters
* (not confirmed)

### MOD inverters
* (not confirmed)

### MID inverters
* (not confirmed)

### MAX inverters
* (not confirmed)

## Requirements
* ESP32
* TTL To RS485 Module with automatic flow control
* or
* KlatremisHW Basic/Lilygo t-can 485, *For now, only danish customers: https://badenergy.dk/product-category/inverter/inverter-styring/

## Installation
1. Create your esp32 in esphome in home assistant
2. Upload the your basis config via. usb from pc.
3. Test wireless upload
4. Copy all content (make sure you have your wifi ssid&password in the secrets)
5. Edit the sensors in the config if you like
6. Upload wireless

## Wiring of generic esp32 & TTL module
RX / TX between esp and ttl converter may have to be swapped. This seems to be a little different from espboard to espboard.
If it dosent communicate(RX/TX led both blinking) Try swap rx/tx on the esp.
 ![image](https://github.com/klatremis/esphome-for-bms/blob/main/wiring.jpg)
