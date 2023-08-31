### Install Prometheus Using Helm

## Add helm repo for Prometheus

```
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
```

## Update Helm Repo

```
helm repo update
```

## install Prometheus using Helm

```
helm install prometheus prometheus-community/prometheus
```

## Expose Prometheus Service 

```
kubectl expose service prometheus-server --type=NodePort --target-port=9090 --name=prometheus-server-ext

```