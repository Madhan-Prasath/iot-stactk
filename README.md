# IOT Stack

## Building

### Pre-requisite:
1. Install Docker-desktop using WSL2 from Windows 10+

### Configurations
## InfluxDB config
Configuration can be done with the influxdb.env file.

## Grafana config
Configuration is done in the grafana.env file. To connect it to the influxdb database the 'influxdb' hostname can be used: http://influxdb:8086

## Node-red
Node red configuration has to be done in the docker volume itself.

## MQTT
The mosquitto configuration has to be done in the docker volume itself.
