# Telegraf

Having Telegraf running in a Docker container means that it can collects metrics which are avaible within it.
To access host metrics configuration in `compose-override.yml` is necessary. See [_Running Telegraf inside a docker container_](https://jacobtomlinson.dev/posts/2016/running-telegraf-inside-a-docker-container/) for details.

## `telegraf.conf`

Add the following configuration for CPU/GPU temperature reporting:

```ini
[[inputs.file]]
  files = ["/sys/class/thermal/thermal_zone0/temp"]
  name_override = "cpu_temperature"
  data_format = "value"
  data_type = "integer"
```
