# smart-home

## MQTT Topic Structure

Since the use of multiple Tasmota-based devices, the [Tasmota MQTT topic structure](https://tasmota.github.io/docs/MQTT/) is applied:

Schema: `%prefix%/<location>/[<floor>|<room>]/hall/%topic%/`

Topics:

- `%prefix%/dresden`
  - `livingroom`
    - `light-switch-1`
  - `hall`
    - `light-switch`
  - `noah`
    - `bed-light-switch`
  - `cellar`
    - `temperature-humidity`
