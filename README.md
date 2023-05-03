# ESPHomeDSMRVictron
Enable readout of a DSMR grid meter and export the data to Home Assistant and a Victron Energy GX device D-Bus

Based on
- https://github.com/hsteinhaus/esph-gadgets/blob/master/esphome/d0-meter.yaml
- https://www.zuidwijk.com/slimmelezer-configuration/

Using and needed on GX-device:
- https://github.com/freakent/dbus-mqtt-devices

## DSMR connection
For the connection and wiring, please see: https://github.com/bartwo/esp32_p1meter#circuit-diagram

## Victron GX integration
To work, this needs
- https://github.com/freakent/dbus-mqtt-devices
- MQTT broker on the Victron controller to be active:
![Victron main view](/images/EnableMQTT.JPG)

If you are not using the Home Assistant part (only MQTT), you must remove the api: line from your ESPHome configuration, otherwise the ESP will reboot every 15 minutes because no client connected to the native API.

I tested this on a Raspberry Pi with Venus OS, but I don't have a Victron setup (yet). The meter shows up like expected, but was not yet tested on a full ESS system:

![Victron main view](/images/overview.JPG)

![Victron main view](/images/Victron_Main.JPG)

![Victron main view](/images/Meter1.JPG)

![Victron main view](/images/meter2.JPG)

![Victron main view](/images/device1.JPG)

![Victron main view](/images/device2.JPG)

I'll maybe add other configs later to add PV inverter data to a GX device via MQTT and Home Assistant. 
