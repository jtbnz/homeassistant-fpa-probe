# 🔥 Fisher & Paykel Appliances BLE Integration

Integrate Fisher & Paykel Appliances Predictive Probes (based on [Combustion](https://combustion.inc) predictive probes) into Home Assistant.

Reuse all the work done by https://github.com/legrego/homeassistant-combustion I am only changing the text fields - all the credit goes to https://github.com/legrego

[![GitHub Release][releases-shield]][releases]
[![License][license-shield]](LICENSE)
![Project Maintenance][maintenance-shield]

**This integration will set up the following platforms.**

Platform | Description
-- | --
`binary_sensor` | Show battery status from probes on your Meatnet.
`sensor` | Show temperature data from probes on your Meatnet.

## Installation

1. Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`).
1. If you do not have a `custom_components` directory (folder) there, you need to create it.
1. In the `custom_components` directory (folder) create a new folder called `combustion`.
1. Download _all_ the files from the `custom_components/combustion/` directory (folder) in this repository.
1. Place the files you downloaded in the new directory (folder) you created.
1. Restart Home Assistant
1. Ensure you have a Combustion device turned on, and within bluetooth range of Home Assistant .
1. In the HA UI go to "Configuration" -> "Integrations" to see your discovered Combustion device.

## Configuration

There is currently no configuration required for this integration. Once the integration discovers your Fisher & Paykel Appliances device(s), it will prompt you to add them on the Integrations page.

## Supported devices

This integration supports reading temperature and battery data from Fisher & Paykel Appliances's [Predictive Thermometer](https://www.fisherpaykel.com/nz/accessories/cooking-accessories/wireless-temperature-sensor-wtsc1-82765.html).

This integration can read data from a probe directly, or via a Meatnet repeater such as the [Range-Extending Booster](https://combustion.inc/products/long-range-predictive-thermometer) or [Range-Extending Display](https://combustion.inc/products/range-extending-display).

This integration will not display information about the repeater itself, only the probes connected to it.

## Contributions are welcome!

If you want to contribute to this please read the [Contribution guidelines](CONTRIBUTING.md)

## Credits

https://github.com/legrego/homeassistant-combustion who credits:

Combustion, Inc. for their wonderful [documentation](https://github.com/combustion-inc/combustion-documentation) and [code samples](https://github.com/combustion-inc/combustion-ios-ble).


***
[Fisher & Paykel Appliances]: https://www.fisherpaykel.com/
[combustion]: https://combustion.inc/
[license-shield]: https://img.shields.io/github/license/legrego/homeassistant-combustion.svg?style=flat
[maintenance-shield]: https://img.shields.io/badge/maintainer-Larry%20Gregory%20@legrego-blue.svg?style=flat
[releases-shield]: https://img.shields.io/github/release/legrego/homeassistant-combustion.svg?style=flat
[releases]: https://github.com/legrego/homeassistant-combustion/releases
