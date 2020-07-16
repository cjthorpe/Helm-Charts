# prometheus-thanos-helm-chart
-------------

Deploys Prometheus along with a Thanos sidecar using a Helm chart.

-------------
## Prerequisites

  - Kubernetes 1.14.9+
  - Helm 3.0+

-------------
## Installing the Chart

Clone the deployment-config repo and run the following command from root.

```console
$ helm upgrade --install --namespace <namespace> --values values.yaml ./charts/prometheus-thanos-sidecar
```

Note it is important that you configure your values file first.

-------------
## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```console
$ helm delete my-release --namespace <namespace>
```
