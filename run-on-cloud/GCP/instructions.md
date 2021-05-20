Connect to GCP and create a GKE cluster
Launch Cloud Shell
Git clone 

    git clone https://github.com/KVSDURGASURESH/kubernetes.git

Run the below command to install/configure kubectl 

    gcloud container clusters get-credentials example-voting-app --zone us-central1-c --project example-voting-app

kubectl get nodes

kubectl create -f deployments/voting-app-deploy.yaml
kubectl create -f service/voting-app-service.yaml
kubectl get all
kubectl create -f deployments/redis-deploy.yaml
kubectl create -f service/redis-service.yaml
kubectl create -f deployments/postgres-deploy.yaml
kubectl create -f service/postgres-service.yaml
kubectl create -f deployments/worker-app-deploy.yaml
kubectl create -f deployments/result-app-deploy.yaml
kubectl create -f service/result-app-service.yaml
kubectl get all




   