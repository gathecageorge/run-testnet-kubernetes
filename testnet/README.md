# testnet launch

```bash
# Bootnode
kubectl apply -f bootnode.yaml

# Config map
# Remember to update bootnode enr before
kubectl apply -f configmap.yaml

# Clients
kubectl apply -f clients/lighthouse.yaml
kubectl apply -f clients/nimbus.yaml
kubectl apply -f clients/prysm.yaml
kubectl apply -f clients/teku.yaml
```
