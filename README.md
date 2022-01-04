# smart-home

## TODOS

- [ ] HA: Why is container not in `iotstack_nw`?
- [ ] HA: Exclude unrelated entities from sync to influx
- [ ] HA: Rename entities for temp/hum sensors

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
