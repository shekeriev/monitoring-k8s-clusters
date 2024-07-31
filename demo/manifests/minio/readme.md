# MinIO Operator and Tenant

A sample set of manifests used to deploy a simple MinIO infrastructure.

As a minimum the **minio-volumes.yaml** file should be adjusted by changing the path for every volume and the target host. 

It is a **mandatory** component. It could be substitued with another S3-compatible solution.

Files:

* [minio-volumes.yaml](minio-volumes.yaml) - a manifest for two persistent volumes that are used by the tenant
* [minio-tenant-values.yaml](minio-tenant-values.yaml) - the custom values to be used with the Helm chart
* [patch-operator-console-service.yaml](patch-operator-console-service.yaml) - a patch that fixes the NodePort of the Operator Console service