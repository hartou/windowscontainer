az acr build --registry $ACR_NAME --image helloacrtasks:v1 --file /path/to/Dockerfile 


az acr build --registry $ACR --image mynet8app:v1 --file Dockerfile


az acr build -t sample/myapp:{{.Run.ID}} -r jrlreg .