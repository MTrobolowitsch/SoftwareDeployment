## Teil 1
# Word Press Anlage
Gruppe anlegen: az group create --name lab3 --location "westeurope"          
Serviceplan anlegen: az appservice plan create --name lab3AppServicePlan --resource-group lab3 --sku S1 --is-linux         
Deployment: az webapp create --resource-group lab3 --plan lab3AppServicePlan --name lab3wordpress --multicontainer-config-type compose --multicontainer-config-file docker-compose-wordpress.yml

Endpoint: https://lab3wordpress.azurewebsites.net/

# Teil 2