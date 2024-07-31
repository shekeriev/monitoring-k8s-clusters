# Cortex

The central and most important component of the whole demo.

It is a **mandatory** component.

Files:

* [cortex-values.yaml](cortex-values.yaml) - the custom values to be used with the Helm chart
* [patch-nginx-service.yaml](patch-nginx-service.yaml) - a patch that fixes the NodePort of the NGINX service
* [patch-querier-service.yaml](patch-querier-service.yaml) - a patch that fixes the NodePort of the Querier service