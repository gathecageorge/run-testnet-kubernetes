# testnet launch

```bash
# Bootnode
kubectl apply -f clients/bootnode.yaml

# Clients
kubectl apply -f clients/lighthouse.yaml
kubectl apply -f clients/nimbus.yaml
kubectl apply -f clients/prysm.yaml
kubectl apply -f clients/teku.yaml
```
