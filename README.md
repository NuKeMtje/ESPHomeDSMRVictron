# ESPHomeDSMRVictron
Enable readout of a DSMR grid meter and export the data to Home Assistant and a Victron Energies GX device D-Bus

Based on
- https://github.com/hsteinhaus/esph-gadgets/blob/master/esphome/d0-meter.yaml
- https://www.zuidwijk.com/slimmelezer-configuration/

Using and needed on GX-device:
- https://github.com/freakent/dbus-mqtt-devices

## DSMR connection
For the connection and wiring, please see: https://github.com/bartwo/esp32_p1meter#circuit-diagram

## Victron GX integration
Remains untested (I don't have an installation yet, but will maybe try on a Raspberry Pi or by a Victron setup in the future).
Needs https://github.com/freakent/dbus-mqtt-devices to work.
