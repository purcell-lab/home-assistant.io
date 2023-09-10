---
title: Tesla Wall Connector
description: Instructions on how to integrate Tesla Wall Connector (Gen 3) into Home Assistant.
ha_category:
  - Binary Sensor
  - Energy
  - Sensor
ha_release: 2021.12
ha_iot_class: Local Polling
ha_config_flow: true
ha_codeowners:
  - '@einarhauks'
ha_domain: tesla_wall_connector
ha_dhcp: true
ha_platforms:
  - binary_sensor
  - sensor
ha_integration_type: integration
---

The Tesla Wall Connector integration allows you to integrate your Gen 3 [Tesla Wall Connector](https://www.tesla.com/support/home-charging-installation/wall-connector) with Wi-Fi into Home Assistant. This integration does not provide visibility of multiple Tesla Wall Connectors that are configured in power sharing mode.

{% include integrations/config_flow.md %}

### Binary Sensor

The following binary sensors are added:

- Contactor closed - Charging/ Not Charging
- State - 1-11 (11 means charging)
- Vehicle connected - Pluggin in/ Unplugged

### Sensor

The following sensors are added:

- Energy - lifetime energy in Wh

### Diagnostic Sensor

The following sensors are added:

- Grid frequency - Hertz (Hz)
- Grid voltage - Volts (V)
- Handle temperature - Degrees Centigrade (°C)/ Degrees Fahrenheit (°F) (127 ° means the handle button has been pressed)
- Phase A/B/C current - Amperes (A)
- Phase A/B/C voltage - Volts (V)

### Switch

This integration does not provide any switches nor control over the unit.

## Device Info

- Serial number
- by Tesla
- Firmware revision
