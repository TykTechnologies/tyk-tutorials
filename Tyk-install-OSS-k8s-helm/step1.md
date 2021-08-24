As you wait for the k8s cluster to start (1-2min) you can also check out the Tyk OSS Helm chart in [ArtifactHUB](https://artifacthub.io/packages/helm/tyk-helm/tyk-headless "ArtifactHUB Tyk OSS Gateway").

When ready, follow the steps below to prepare your cluster for installation:

*  Add the Tyk official Helm repo

`helm repo add tyk-helm https://helm.tyk.io/public/helm/charts/`{{execute}}

*  Update the repo for the latest information from the chart repositories as information is cached locally.

`helm repo update`{{execute}}

*  Although not essential, we do recommend creating a namespace for your Tyk deployment

`kubectl create namespace tyk`{{execute}}
