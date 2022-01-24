# Webapp Deploy Demo with Deployment Center


Create an Azure App Service Plan (Linux Flavor) and App Service for Python 3.9

```shell
az group create --name webapp-github-deployment --location westeurope
az appservice plan create -g webapp-github-deployment -n webapp-github-deployment --is-linux
az webapp create -g webapp-github-deployment -n webapp-github-deploy-demo -p webapp-github-deployment --runtime "PYTHON|3.9"
```
