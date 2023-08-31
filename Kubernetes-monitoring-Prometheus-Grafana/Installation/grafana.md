### Install Grafana using Helm

## Add the Helm Repo

```
helm repo add grafana https://grafana.github.io/helm-charts
```

## Update Helm Repo [To get latest updates]

```
helm repo update
```

## Install Grafana using Helm

```
helm install grafana grafana/grafana
```

## Expose Grafana Service

```
kubectl expose service grafana — type=NodePort — target-port=3000 — name=grafana-ext
```