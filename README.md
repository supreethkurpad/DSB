# DeathStarBench

Open-source benchmark suite for cloud microservices. DeathStarBench includes five end-to-end services, four for cloud systems, and one for cloud-edge systems running on drone swarms. 

This is a fork of the official DeathStarBench repository. Modifications have been made to convert the nginx-thrift service to a NodePort service so it can be accessed through the IP address of the node without port forwarding.

# Steps to deploy the application on Kubernetes
Once the Kubernetes cluster is setup correctly, running the below command will deploy the application.
```
helm install v1 socialNetwork/helm-chart/socialnetwork
```
The application can be accessed on <IP>:31111
The port for the same can be configured in the following file: `socialNetwork/helm-chart/socialnetwork/charts/nginx-thrift/values.yaml`
