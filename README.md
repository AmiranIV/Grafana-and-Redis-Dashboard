## Deploy a Grafana server with Redis integration that presents information about the redis-cart DB

## provisioned in the cluster as part of the Online Boutique Service ( I will attach later on)

- Create a secret Before the deployment using this command:

kubectl create secret generic grafana-admin-password --from-literal='admin-user=<YOURNAME>' --from-literal='admin-pass=<YOURPASSWORD>'

The name and password are your choice.

<img width="1355" alt="Screenshot 2023-12-19 at 15 35 18" src="https://github.com/AmiranIV/Grafana-and-Redis-Dashboard/assets/109898333/df0620ed-5ddd-47cb-be3f-9284f5beaa47">
