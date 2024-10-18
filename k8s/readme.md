How to setup two-tier application deployment on kubernetes cluster
First setup kubernetes kubeadm cluster
Use this repository to setup kubeadm https://github.com/LondheShubham153/kubestarter/blob/main/kubeadm_installation.md

SetUp
First clone the code to your machine
git clone https://github.com/LondheShubham153/two-tier-flask-app.git
Move to k8s directory
cd two-tier-flask-app/k8s
Now, execute below commands one by one
kubectl apply -f twotier-deployment.yml
kubectl apply -f twotier-deployment-svc.yml
kubectl apply -f mysql-deployment.yml
kubectl apply -f mysql-deployment-svc.yml
kubectl apply -f persistent-volume.yml
kubectl apply -f persistent-volume-claim.yml
