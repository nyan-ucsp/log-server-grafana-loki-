# Log Server With Grafana & Loki

### Grafana
Grafana is an open-source platform that specializes in data visualization and monitoring.

### Loki
Grafana Loki is a log storage system built by Grafana that works alongside Grafana for visualization. It efficiently stores and retrieves logs from your applications, allowing you to search and analyze them using a powerful query language.

## How to start this system
**prerequisite:** Docker

#### Build Log Server
```
docker compose build
```

#### Create Log Container
```
docker compose create
```

#### Start Log Server
```
docker compose start
```

## Run your Log Server

### Grafana Dashboard

You can find Grafana Dashboard at http://localhost:3000

username: **admin**

password: **minmin**

### Test Loki

You can check your loki is running or not with this link
http://localhost:3100/ready

First Loki response is **Ingester not ready: waiting for 15s after being ready**

Retry After 15s output is **ready**