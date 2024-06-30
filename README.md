## About
This is a GitHub repository for the `values.yaml` file used for the Medium articles about multi-cluster monitoring solution using Thanos, Grafana and Prometheus.

You can find the articles here: 
- [Theory — Monitoring with Prometheus & Thanos [Part 1/2]](https://medium.com/@dast04/theory-monitoring-with-prometheus-thanos-part-1-2-8bc500a9c6a8)
- [Deployment — Monitoring with Prometheus & Thanos [Part 2/2]](https://medium.com/@dast04/full-installation-monitoring-with-prometheus-thanos-part-2-2-fe98fcdbe448)


## Deployment of the chart

```bashrc
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update
```

```bashrc
helm upgrade --install monitoring prometheus-community/kube-prometheus-stack \
    --namespace monitoring \
    --values values.yaml \
    --version "60.2.0"
```
