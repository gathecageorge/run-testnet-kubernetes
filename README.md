# ReadMe

## setup for all

```bash
# Create linode PVC if not exists only
kubectl apply -f storage/pvc.yaml

# Setup NFS server if not setup
kubectl apply -f storage/nfs.yaml

# Configure persistent volume from NFS server to be shared.
# Remember to change IP to NFS service IP
kubectl apply -f storage/shared-storage.yaml

# Test storage
kubectl apply -f ubuntu.yaml

# Reset
kubectl delete -f ubuntu.yaml && kubectl delete -f storage/shared-storage.yaml && kubectl delete -f storage/nfs.yaml

# Delete PVC if needed
kubectl delete -f storage/pvc.yaml
```
