### Install chaos-toolkit

python3 -m venv ~/.venvs/chaos
502  source  ~/.venvs/chaos/bin/activate
pip install -U chaostoolkit

(Configure kube config to connect to your K8S cluster)

### Running a single pod
kubectl apply -f pod_nginx.yaml

### Creating a deployment
kubectl apply -f deployment_nginx.yaml

### Run chaos experiment
chaos run chaos-demo.yaml