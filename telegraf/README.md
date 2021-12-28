# Telegraf

## `telegraf.conf`

Add the following configuration for CPU/GPU temperature reporting:

```ini
[[inputs.file]]
  files = ["/sys/class/thermal/thermal_zone0/temp"]
  name_override = "cpu_temperature"
  data_format = "value"
  data_type = "integer"
```