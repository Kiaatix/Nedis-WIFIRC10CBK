# Nedis-WIFIRC10CBK
Nedis WIFIRC10CBK Board

Chip: bk7231n


<img width="300" height="300" alt="Back" src="https://github.com/user-attachments/assets/9f0bbf1b-0389-4a80-bb60-bc6cb0e5ffe5" />

<img width="300" height="300" alt="Front" src="https://github.com/user-attachments/assets/306765ea-7868-4333-94ea-f03a45569045" />

## Pins:
- LED
```
status_led:
  pin: P9
```
- Transmitter:
```
remote_transmitter:
  pin: P7
  carrier_duty_percent: 50%
```
- Receiver:
```
remote_receiver:
  pin:
    number: "P8"
    inverted: true
    mode: INPUT_PULLUP
```
- Button:
```
binary_sensor:
  - platform: gpio
    name: Restart GPIO
    pin:
      number: P23
      mode:
        input: true
        pulldown: true
```
