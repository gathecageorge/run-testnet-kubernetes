# monitoring

This will allow collecting metrics and logs from all pods with label `app: testnet`

The logs are collected using promtail/loki

The metrics are collected using prometheus

There is grafana for viewing the logs/metrics

```bash
# Setup
kubectl apply -f monitoring/main.yaml && kubectl apply -f monitoring/logging.yaml && kubectl apply -f monitoring/metrics.yaml

# Reset
kubectl delete -f monitoring/main.yaml && kubectl delete -f monitoring/logging.yaml && kubectl delete -f monitoring/metrics.yaml
```
