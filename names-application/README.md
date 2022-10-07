# names application

This launches a sample application developed using node js. The application can be found here <https://github.com/gathecageorge/node-names-application>

This will launch a mysql database and then 2 instances of the application.

```bash
# Create
kubectl apply -f names-application/names-application.yaml

# Reset
kubectl delete -f names-application/names-application.yaml
```
