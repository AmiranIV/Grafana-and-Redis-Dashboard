## Deploy a Grafana server with Redis integration that presents information about the redis-cart DB

### provisioned in the cluster as part of the Online Boutique Service of Google Cloud Platform

link to the entire repo that this Deployment is based on: https://github.com/GoogleCloudPlatform/microservices-demo

- Create a secret Before the deployment using this command:

kubectl create secret generic grafana-admin-password --from-literal='admin-user=<YOURNAME>' --from-literal='admin-pass=<YOURPASSWORD>'

The name and password are your choice.

- create the Deployment on one YAML file Deployment + Service file using one command:

kubectl apply -f grafana-Deployment+Service.yaml

I Deployed it on an EC2 so don't forget to port forward using this command if you're on a remote machine as well:

kubectl port-forward service/my-grafana 3000:3000 --address 0.0.0.0


<img width="1355" alt="Screenshot 2023-12-19 at 15 35 18" src="https://github.com/AmiranIV/Grafana-and-Redis-Dashboard/assets/109898333/df0620ed-5ddd-47cb-be3f-9284f5beaa47">
