# Local Prometheus Instances

Those are deployed on the workload clusters.

The address of the Cortext endpoint used for ***remote write*** **MUST** be changed to match the address in the actual setup. The current value is a placeholder ***http://\<the-ip-address-of-jupiter-control-plane\>:30123/api/v1/push***

These are **mandatory** components.

Files:

* [kube-prometheus-stack-values-tenant-cluster-mars.yaml](kube-prometheus-stack-values-tenant-cluster-mars.yaml) - the custom values for the **first workload cluster** (**Mars**) to be used with the Helm chart
* [kube-prometheus-stack-values-tenant-cluster-venus.yaml](kube-prometheus-stack-values-tenant-cluster-venus.yaml) - the custom values for the **second workload cluster** (**Venus**) to be used with the Helm chart
* [metrics-proxy.yaml](metrics-proxy.yaml) - a manifest for a proxy to make the system components reachable by the respective Prometheus instance