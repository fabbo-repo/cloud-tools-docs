### Create a cluster for running containers [MORE](https://cloud.google.com/sdk/gcloud/reference/container/clusters/create)
~~~
gcloud container clusters create <CLUSTER_NAME>
~~~

### Setup local Kubeconfig with remote cluster
~~~
gcloud container clusters get-credentials <CLUSTER_NAME> --zone <ZONE> --project <PROJECT_ID>
~~~