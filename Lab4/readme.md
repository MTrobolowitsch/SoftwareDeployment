## Commands
az group create --name AKS --location westeurope
az aks create --resource-group lab4 --name myAKSCluster --node-count 1 --enable-addons monitoring --generate-ssh-keys


## Link zur wordpress
http://20.73.37.199/ => Externe IP von Loadbalance

## kustomization.yaml
Beinhaltet die Ressourcen (Wordpress und MySQL)

## mysql-deployment.yaml
Die YAML Datei beinhaltet das MySQL Deployment mit einem persistent volume auf /var/lib/mysql.

# Deployment triggern
kubectl apply -k ./