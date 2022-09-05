# ff-pushpin-service

![Version: 0.2.3](https://img.shields.io/badge/Version-0.2.3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.1](https://img.shields.io/badge/AppVersion-0.0.1-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://harness.github.io/helm-common | harness-common | 1.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| appLogLevel | string | `"INFO"` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| configmap | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| global.airgap | bool | `false` |  |
| global.ha | bool | `false` |  |
| global.ingress.className | string | `"nginx"` |  |
| global.ingress.enabled | bool | `false` |  |
| global.ingress.hosts[0] | string | `"my-host.example.org"` |  |
| global.ingress.tls.enabled | bool | `false` |  |
| global.ingress.tls.secretName | string | `"harness-ssl"` |  |
| global.loadbalancerURL | string | `"test@harness.io"` |  |
| maxSurge | int | `1` |  |
| maxUnavailable | int | `0` |  |
| memory | int | `4096` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| pushpin.image.digest | string | `""` |  |
| pushpin.image.pullPolicy | string | `"IfNotPresent"` |  |
| pushpin.image.registry | string | `"docker.io"` |  |
| pushpin.image.repository | string | `"harness/ff-pushpin-signed"` |  |
| pushpin.image.tag | string | `"1.546.0"` |  |
| pushpin.resources.limits.cpu | int | `1` |  |
| pushpin.resources.limits.memory | string | `"2048Mi"` |  |
| pushpin.resources.requests.cpu | int | `1` |  |
| pushpin.resources.requests.memory | string | `"2048Mi"` |  |
| pushpinworker.image.digest | string | `""` |  |
| pushpinworker.image.pullPolicy | string | `"IfNotPresent"` |  |
| pushpinworker.image.registry | string | `"docker.io"` |  |
| pushpinworker.image.repository | string | `"harness/ff-pushpin-worker-signed"` |  |
| pushpinworker.image.tag | string | `"1.546.0"` |  |
| pushpinworker.resources.limits.cpu | int | `1` |  |
| pushpinworker.resources.limits.memory | string | `"2048Mi"` |  |
| pushpinworker.resources.requests.cpu | int | `1` |  |
| pushpinworker.resources.requests.memory | string | `"2048Mi"` |  |
| pushpinworker.securityContext.runAsNonRoot | bool | `true` |  |
| pushpinworker.securityContext.runAsUser | int | `65534` |  |
| replicaCount | int | `1` |  |
| service.port17001 | int | `17001` |  |
| service.port17002 | int | `17002` |  |
| service.port17002 | int | `17003` |  |
| service.targetport17001 | int | `7999` |  |
| service.targetport17002 | int | `443` |  |
| service.targetport17003 | int | `5561` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `"harness-default"` |  |
| tolerations | list | `[]` |  |

