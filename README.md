# testnet launch

```bash
# Setup Storage before everything
kubectl apply -f local-storage.yaml

# Bootnode
kubectl apply -f clients/bootnode.yaml

# Clients
kubectl apply -f clients/lighthouse.yaml && kubectl apply -f clients/nimbus.yaml && kubectl apply -f clients/prysm.yaml && kubectl apply -f clients/teku.yaml

# Delete clients
kubectl delete -f clients/lighthouse.yaml && kubectl delete -f clients/nimbus.yaml && kubectl delete -f clients/prysm.yaml && kubectl delete -f clients/teku.yaml
```
