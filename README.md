[![verified-by-homebridge](https://badgen.net/badge/homebridge/verified/purple)](https://github.com/homebridge/homebridge/wiki/Verified-Plugins)
[![npm-version](https://badgen.net/npm/v/homebridge-adguardhome)](https://www.npmjs.com/package/homebridge-adguardhome)
[![npm-total-downloads](https://badgen.net/npm/dt/homebridge-adguardhome)](https://www.npmjs.com/package/homebridge-adguardhome)

<p align="center">
<img src="https://github.com/homebridge/branding/raw/master/logos/homebridge-wordmark-logo-vertical.png" width="150">
</p>

# Homebridge AdGuard Home

Display AdGuard Home as a lock accesory.

NOTE: When updating from 1.5.1 to 1.6.0 you might need to re-add the accessory again.

## Requirements

- [Homebridge](https://github.com/nfarina/homebridge) HomeKit support for the impatient
- [AdGuard Home](https://github.com/AdguardTeam/AdGuardHome) Network-wide ads & trackers blocking DNS server

## Example config

```json
{
  "bridge": {
    "name": "Homebridge",
    "username": "CC:22:3D:E3:CE:30",
    "port": 51826,
    "pin": "031-45-154"
  },
  "accessories": [
    {
      "accessory": "AdGuardHome",
      "name": "AdGuard",
      "username": "ADGUARD_USERNAME",
      "password": "ADGUARD_PASSWORD",
      "host": "192.168.1.2",
      "https": false,
      "Type": "LOCK" // default: "SWITCH"
    }
  ]
}
```
