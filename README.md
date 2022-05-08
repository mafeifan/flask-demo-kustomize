# flask-demo-kustomize
gitops of flask demo with kustomize

```
# 集群安装controller
kubectl apply -f https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.17.5/controller.yaml

# 安装客户端
wget https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.17.5/kubeseal-0.17.5-linux-amd64.tar.gz
kubeseal --scope cluster-wide --format=yaml --cert .public-cert.pem < secret.yaml > secret-seal.yaml
```
