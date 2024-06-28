# Thanos_prometheus


helm upgrade --install $RELEASE_NAME prometheus-community/kube-prometheus-stack \
    --namespace $NAMESPACE \
    --values values.yaml \
    --version "60.2.0"
