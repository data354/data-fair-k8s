### Prerequis
- Avoir minikube, kubectl installés

## 1- Créer un namespace
     kubectl create namespace data-fair
## 2- Activer le namespace
     kubectl config set-context --current --namespace data-fair

## 3- Déployer les applications
     kubectl apply -f services
     kubectl apply -f config
     kubectl apply -f data
     kubectl apply -f app
     
## 4- Récuperer les services
     minikube service --all -n data-fair

## 5- Lancer le service nginx avec son url