# Creation app in production with a loadbalancer (nodePort) which switch between pods
## Creation namespace production
* kubectl create -f ./my-namespace.yaml
## Creation Service (implicit loadbalancer)
* kubectl apply -f service-nodeport-web.yml
* kubectl -n production get svc
* kubectl describe svc service-nodeport-web -n production