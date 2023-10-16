# ESPhome for deye (still under development)
ESPhome configuration for monitoring and control of Growatt inverters in Home Assistant.
This include all addresses i could see relevant from the inverter.

## Supported devices
Made specially for Growatt inverters

### SPH inverters
* SPH3600 (not confirmed)
* SPH8000TL3 (not confirmed)
### MOD inverters
* Comming soon

## Requirements
* ESP32 with TTL To RS485 Module with automatic flow control
* Or Lilygo t-can485 board

## Installation
1. Create your esp32 in esphome in home assistant
2. Upload the your basis config via. usb from pc.
3. Test wireless upload
4. Copy all content (make sure you have your wifi ssid&password in the secrets)
5. Edit the sensors in the config if you like
6. Upload wireless

## Hardware diagram
RX / TX between esp and ttl converter way have to be swapped. This seems to be a little different from espboard to espboard.
If it dosent communicate(RX/TX led both blinking) Try swap rx/tx on the esp.
