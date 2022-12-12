# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
![Screenshot](DockerImages.jpg)
* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
![Screenshot](TravisCI-Integration.jpg)
* Travis CI showing a successful build and deploy job
![Screenshot](TravisCI_Successful.jpg)
## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![Screenshot](Pods.jpg)
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![Screenshot](services-1.jpg)
![Screenshot](service-2.jpg)

To verify that you have set up services to loadbalancer
kubectl get services
![Screenshot](services.jpg)

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![Screenshot](hpa.jpg)
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![Screenshot](Feed-API-Logs.jpg)
![Screenshot](User-API-Logs.jpg)

AWS Screenshots

![Screenshot](AWS-Cluster.jpg)
![Screenshot](AWS-Cluster-Nodes.jpg)
![Screenshot](AWS-RDS.jpg)
![Screenshot](AWS-S3Bucket.jpg)