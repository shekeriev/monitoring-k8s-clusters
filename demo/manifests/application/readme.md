# Dummy Application and ServiceMonitor

This is a dummy Go-based web application. It is used to illustrate how application metrics can be collected and used. 

It is an **optional** component.

Files:

* [promgraf.yaml](promgraf.yaml) - application's manifest that contains definitions of a pod and service
* [service-monitor.yaml](service-monitor.yaml) - service monitor manifest to register the application in the respective Prometheus instance