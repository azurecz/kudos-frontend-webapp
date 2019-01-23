# kudos-frontend-webapp
WebApp serving front end

# Deploy complete solution from master template
Go to kudos repo and use master template to provision all components of the solution.

# Deploy SPA frontend via portal
Click button and follow wizard.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fgithub.com%2Fazurecz%2Fkudos-frontend-webapp%2Fraw%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

# Deploy SPA frontend from GitHub
```
az group create -n kudos -l westeurope
az group deployment create -g kudos \
    --template-uri https://github.com/azurecz/kudos-frontend-webapp/raw/master/azuredeploy.json
```

# Deploy SPA frontend from local
```
az group create -n kudos -l westeurope
az group deployment create -g kudos --template-file azuredeploy.json
```