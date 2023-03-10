# capd

![Version: 1.3.3](https://img.shields.io/badge/Version-1.3.3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.3.3](https://img.shields.io/badge/AppVersion-1.3.3-informational?style=flat-square)

A Helm Chart for the cluster-api infrastructure provider

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| controllerManager.manager.image.repository | string | `"gcr.io/k8s-staging-cluster-api/capd-manager"` |  |
| controllerManager.manager.image.tag | string | `"v1.3.3"` |  |
| controllerManager.replicas | int | `1` |  |
| kubernetesClusterDomain | string | `"cluster.local"` |  |
| providerArgs.clusterTopology | bool | `false` |  |
| providerArgs.machinePool | bool | `false` |  |
| webhookService.ports[0].port | int | `443` |  |
| webhookService.ports[0].targetPort | string | `"webhook-server"` |  |
| webhookService.type | string | `"ClusterIP"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
