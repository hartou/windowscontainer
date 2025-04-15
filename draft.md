# Corrected Azure CLI commands for building container images

# Build and push the helloacrtasks:v1 image to the specified Azure Container Registry
az acr build --registry $ACR_NAME --image helloacrtasks:v1 --file ./path/to/Dockerfile .

# Build and push the mynet8app:v1 image to the specified Azure Container Registry
az acr build --registry $ACR --image mynet8app:v1 --file ./MyNet8App/Dockerfile .

# Build and push the sample/myapp image with a unique tag to the specified Azure Container Registry
az acr build --image sample/myapp:{{.Run.ID}} --registry jrlreg --file ./Dockerfile