The app can be tested using minikube cluster. Build the docker app locally

- docker build -t kata-app:demo .

Create namespace and deploy the app with service in minikube cluster

- kubectl create ns kata-app
- kubectl apply -f deployment.yaml
- kubectl apply -f service.yaml

Get minikube IP
- minikube ip

Then, access your app at:
- http://<minikube-ip>:30007/
