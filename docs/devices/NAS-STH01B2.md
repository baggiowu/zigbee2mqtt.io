---
title: "NEO NAS-STH01B2 control via MQTT"
description: "Integrate your NEO NAS-STH01B2 via Zigbee2MQTT with whatever smart home infrastructure you are using without the vendor's bridge or gateway."
addedAt: 
pageClass: device-page
---

<!-- !!!! -->
<!-- ATTENTION: This file is auto-generated through docgen! -->
<!-- You can only edit the "Notes"-Section between the two comment lines "Notes BEGIN" and "Notes END". -->
<!-- Do not use h1 or h2 heading within "## Notes"-Section. -->
<!-- !!!! -->

# NEO NAS-STH01B2

|     |     |
|-----|-----|
| Model | NAS-STH01B2  |
| Vendor  | [NEO](/supported-devices/#v=NEO)  |
| Description | Soil moisture and temperature |
| Exposes | humidity, temperature, temperature_f, temperature_sensitivity, humidity_sensitivity, temperature_alarm, humidity_alarm, max_temperature_alarm, min_temperature_alarm, max_humidity_alarm, min_humidity_alarm, schedule_periodic, battery_percentage, linkquality |
| Picture | ![NEO NAS-STH01B2](https://www.zigbee2mqtt.io/images/devices/NAS-STH01B2.png) |


<!-- Notes BEGIN: You can edit here. Add "## Notes" headline if not already present. -->


<!-- Notes END: Do not edit below this line -->



## Options
*[How to use device type specific configuration](../guide/configuration/devices-groups.md#specific-device-options)*

* `humidity_calibration`: Calibrates the humidity value (absolute offset), takes into effect on next report of device. The value must be a number.

* `humidity_precision`: Number of digits after decimal point for humidity, takes into effect on next report of device. This option can only decrease the precision, not increase it. The value must be a number with a minimum value of `0` and with a with a maximum value of `3`

* `temperature_calibration`: Calibrates the temperature value (absolute offset), takes into effect on next report of device. The value must be a number.

* `temperature_precision`: Number of digits after decimal point for temperature, takes into effect on next report of device. This option can only decrease the precision, not increase it. The value must be a number with a minimum value of `0` and with a with a maximum value of `3`


## Exposes

### Humidity (numeric)
Soil humidity.
Value can be found in the published state on the `humidity` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `0` and the maximum value is `100`.
The unit of this value is `%`.

### Temperature (numeric)
Soil temperature.
Value can be found in the published state on the `temperature` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `-10` and the maximum value is `60`.
The unit of this value is `°C`.

### Temperature f (numeric)
Soil temperature.
Value can be found in the published state on the `temperature_f` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `14` and the maximum value is `140`.
The unit of this value is `°F`.

### Temperature sensitivity (numeric)
Upper temperature limit.
Value can be found in the published state on the `temperature_sensitivity` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"temperature_sensitivity": NEW_VALUE}`.
The minimal value is `0.3` and the maximum value is `1`.
The unit of this value is `°C`.

### Humidity sensitivity (numeric)
Upper temperature limit.
Value can be found in the published state on the `humidity_sensitivity` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"humidity_sensitivity": NEW_VALUE}`.
The minimal value is `1` and the maximum value is `5`.
The unit of this value is `%`.

### Temperature alarm (enum)
Temperature alarm state.
Value can be found in the published state on the `temperature_alarm` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The possible values are: `lower_alarm`, `upper_alarm`, `cancel`.

### Humidity alarm (enum)
Humidity alarm state.
Value can be found in the published state on the `humidity_alarm` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The possible values are: `lower_alarm`, `upper_alarm`, `cancel`.

### Max temperature alarm (numeric)
Upper temperature limit.
Value can be found in the published state on the `max_temperature_alarm` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"max_temperature_alarm": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `60`.
The unit of this value is `°C`.

### Min temperature alarm (numeric)
Lower temperature limit.
Value can be found in the published state on the `min_temperature_alarm` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"min_temperature_alarm": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `60`.
The unit of this value is `°C`.

### Max humidity alarm (numeric)
Upper humidity limit.
Value can be found in the published state on the `max_humidity_alarm` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"max_humidity_alarm": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `100`.
The unit of this value is `%`.

### Min humidity alarm (numeric)
Lower humidity limit.
Value can be found in the published state on the `min_humidity_alarm` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"min_humidity_alarm": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `100`.
The unit of this value is `%`.

### Schedule periodic (numeric)
Report sensitivity.
Value can be found in the published state on the `schedule_periodic` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"schedule_periodic": NEW_VALUE}`.
The minimal value is `5` and the maximum value is `60`.
The unit of this value is `min`.

### Battery percentage (numeric)
Battery percentage.
Value can be found in the published state on the `battery_percentage` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `0` and the maximum value is `100`.
The unit of this value is `%`.

### Linkquality (numeric)
Link quality (signal strength).
Value can be found in the published state on the `linkquality` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `0` and the maximum value is `255`.
The unit of this value is `lqi`.

