# Microservice01
Microservice Testbed



Run Docker Image
docker run -it --rm -p 3000:80 --name microservice01container microservice01


Deploy to Azure
az aks create --resource-group Microservice01Resources --name Microservice01Cluster --node-count 1 --enable-addons http_application_routing --generate-ssh-keys

az aks get-credentials --resource-group Microservice01Resources --name Microservice01Cluster