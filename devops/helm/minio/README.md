## definition

## deploy
```
helm upgrade -i minio-operator minio-operator/operator   --namespace test-everything   --values values.yaml
```

## get jwt console
```
kubectl -n test-everything get secret console-sa-secret -o jsonpath="{.data.token}" | base64 --decode
```
