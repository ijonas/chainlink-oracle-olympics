# chainlink-oracle-olympics
GCP / GKE Infrastructure config files for Chainlink Oracle Olympics



## Setup Chainlink Node API secrets

    kubectl create secret generic api-env --from-file=./secrets/prod/.api    
    kubectl create secret generic password-env --from-file=./secrets/prod/.password

## Add Ingress to Docker-Desktop Kubernetes

    helm install --namespace kube-system nginx ingress-nginx --repo https://kubernetes.github.io/ingress-nginx
