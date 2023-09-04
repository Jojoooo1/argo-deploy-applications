# Argo data personal labs

## Data applications

Available Applications:

| Applications  | DNS | Username  | Password | Links |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Clickhouse | <https://clickhouse.local.com.br/play?user=admin> | admin | password | <https://clickhouse.com> |
| Postgres | postgres.postgres.svc.cluster.local - database: postgres | admin | password | <https://www.postgresql.org> |
| Dbeaver | <dbeaver.local.com.br> | cbadmin | cbadmin20 | <https://dbeaver.com/docs/cloudbeaver> |

## ArgoCD Folders organization

### Base

- **base/applications-data**: Contains k8s observability applications

### Overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.

### Limitations

- open issue working with clickhouse keeper <https://github.com/bitnami/charts/issues/15935>
