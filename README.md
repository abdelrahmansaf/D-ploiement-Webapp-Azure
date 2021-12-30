# D-ploiement-Webapp-Azure

for deploying a build in a zip file using your powershell command line


az appservice plan create --name myAppPlan --resource-group myRG --sku B1 

az webapp create --name myWebAppName --resource-group myRG --plan myAppPlan --runtime "DOTNET:5.0" 

az webapp deploy --resource-group myRG --name myWebAppName --src-path .\myZip.zip --type zip 

az webapp up --name myWebAppName --resource-group myRG
