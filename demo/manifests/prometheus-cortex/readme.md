# Prometheus Instance for Cortex

This is **optional**. It could be deployed to get access to the metrics of the Cortex components.

As a first step, the latest operator bundle manifest should be downloaded:

```bash
curl -s https://raw.githubusercontent.com/prometheus-operator/prometheus-operator/main/bundle.yaml -o prometheus-operator-latest-bundle.yaml
```

*Note: On Windows execute **curl.exe** instead of just ***curl**.**

Files:

* [prometheus-cortex.yaml](prometheus-cortex.yaml) - a set of resources that will allow monitoring of the Cortex installation
* *prometheus-operator-latest-bundle.yaml* - a manifest for the Prometheus operator. This one is **not included** and has to be downloaded as per the instruction above