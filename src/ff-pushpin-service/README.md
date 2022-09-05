# ff-pushpin-service

![Version: 0.2.1](https://img.shields.io/badge/Version-0.2.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.1](https://img.shields.io/badge/AppVersion-0.0.1-informational?style=flat-square)

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
| image.digest | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"harness/ff-pushpin-server-signed"` |  |
| image.tag | string | `"1.546.0"` |  |
| jobs.postgres_migration.image.digest | string | `""` |  |
| jobs.postgres_migration.image.pullPolicy | string | `"Always"` |  |
| jobs.postgres_migration.image.registry | string | `"docker.io"` |  |
| jobs.postgres_migration.image.repository | string | `"harness/ff-pushpin-postgres-migration-signed"` |  |
| jobs.postgres_migration.image.tag | string | `"1.546.0"` |  |
| jobs.timescaledb_migrate.image.digest | string | `""` |  |
| jobs.timescaledb_migrate.image.pullPolicy | string | `"Always"` |  |
| jobs.timescaledb_migrate.image.registry | string | `"docker.io"` |  |
| jobs.timescaledb_migrate.image.repository | string | `"harness/ff-pushpin-timescale-migration-signed"` |  |
| jobs.timescaledb_migrate.image.tag | string | `"1.546.0"` |  |
| maxSurge | int | `1` |  |
| maxUnavailable | int | `0` |  |
| memory | int | `4096` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | int | `1` |  |
| resources.limits.memory | string | `"2048Mi"` |  |
| resources.requests.cpu | int | `1` |  |
| resources.requests.memory | string | `"2048Mi"` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `65534` |  |
| service.grpcport | int | `16002` |  |
| service.port | int | `17001` |  |
| service.targetgrpcport | int | `3001` |  |
| service.targetport | int | `3000` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `"harness-default"` |  |
| timescaleSecret.password.key | string | `"timescaledbPostgresPassword"` |  |
| timescaleSecret.password.name | string | `"harness-secrets"` |  |
| tolerations | list | `[]` |  |

