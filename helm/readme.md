# Helm v3 app
The goal is to deploy easily a wordpress app with its db using helm

## Helm installation
```console
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3
chmod 700 get_helm.sh
yum install openssl -y
./get_helm.sh
helm version
```

# Deployment WordPress
helm repo add bitnami https://charts.bitnami.com/bitnami
helm install wordpress bitnami/wordpress -f ./values.yml

# Useful link
https://devopscube.com/install-configure-helm-kubernetes/