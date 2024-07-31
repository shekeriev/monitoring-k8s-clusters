# Load Generators for the Application and the Clusters

These are **optional**. They could be deployed to simulate some activity.

Files:

* [application-load-generator.yaml](application-load-generator.yaml) - a manifest for a load generator used to simulate activity on the application
* [cluster-workload-preparation.yaml](cluster-workload-preparation.yaml) - a manifest for preparing the environment for the cluster workload set of utilities. Contains service account, role, and binding
* [cluster-workload-generator.yaml](cluster-workload-generator.yaml) - a manifest for the actual cluster workload generator used to simulate activity on the cluster
* [cluster-workload-cleaner.yaml](cluster-workload-cleaner.yaml) - a manifest for a cron job that cleans all the completed pods that are leftovers from the workload generator