# Azure ARM - Example
```sh
# Create Ressource Group
az group create --name testrg --location germanywestcentral

# Apply ARM-Deployment-Template
az group deployment create -g testrg --template-file ./azuredeploy.json --name test

# Delete Deployment
az group deployment delete --name test \
                           --resource-group testrg \
                           --no-wait


# Delete RG
az group delete --name testrg 


```