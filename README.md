## Helm Charts for VP Kuljetus TMS
This repository is part of a VP Kuljetus TMS -project

### Note: RabbitMQ Cluster Operator is not installed together with vp-kuljetus-transport-management-charts 

Installation on a VP-Kuljetus cluster

### Installing RabbitMQ Cluster Operator in a ```rabbit-system``` namespace:

Start with adding a helm chart and installing it:
```
helm repo add bitnami https://charts.bitnami.com/bitnami
kubectl create namespace rabbit-system
helm install rabbitmq-cluster-operator bitnami/rabbitmq-cluster-operator --namespace rabbit-system
```