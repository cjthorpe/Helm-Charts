# cert-manager-helm-chart
-------------

Deploys Jetstack's cert-manager using a Helm chart.

-------------
## Prerequisites

  - Kubernetes 1.15.11+
  - Helm 3.0+

-------------
## Installing the Chart

Clone the cert-manager-helm-chart repo and run the following commands from the root of the repository:

```console
$ helm package ./cert-manager/
```

Depending on the chart version designated in `Chart.yaml` this will produce a package archive file which will be used for the upgrade/installation.

Provide a values file that targets the environment to be deployed to - either Prod or Staging:

```console
$ helm upgrade --install cert-manager ./cert-manager-1.0.0.tgz --values ./cert-manager/values.yaml --debug -n cert-manager
```

Note it is important that you configure your values file first.

-------------
## Uninstalling the Chart

To uninstall the `cert-manager` deployment:

```console
$ helm uninstall cert-manager --namespace cert-manager
```
