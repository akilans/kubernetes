-listen-client-urls http://127.0.0.1:4001,http://172.16.6.4:4001 -advertise-client-urls http://172.16.6.4:4001 ./etcd -listen-client-urls http://127.0.0.1:4001,http://172.16.6.4:4001 -advertise-client-urls http://172.16.6.4:4001
clear
systemctl start kube-apiserver
systemctl start kube-controller-manager
systemctl start kube-scheduler
systemctl start kube-proxy
systemctl start kubelet
systemctl status kube-apiserver
systemctl status kube-controller-manager
systemctl status kube-scheduler
systemctl status kube-proxy
systemctl status kubelet
clear
kubectl get pods
kubectl get namespaces
scp /home/akilan/kube-test/kubernetes.tar.gz root@172.16.6.5:/home/akilan/kube-test/
ls ~/.ssh/
ssh-copy-id -i ~/.ssh/id_rsa.pub root@172.16.6.5
ssh-keygen -f "/root/.ssh/known_hosts" -R 172.16.6.5
ssh-copy-id -i ~/.ssh/id_rsa.pub root@172.16.6.5
scp /home/akilan/kube-test/kubernetes.tar.gz root@172.16.6.5:/home/akilan/kube-test/
scp /home/akilan/kube-test/v1.3.0.tar.gz  root@172.16.6.5:/home/akilan/kube-test/
cat /home/akilan/kube-test/kubernetes/cluster/ubuntu/download-release.sh 
kubectl get pods
docker ps -a
docker ps
kubectl get pods
clear
kubectl get nodes
docker ps
kubectl get namespaces
kubectl get pods --namespace=kube-system
kubectl get sv
kubectl get 
kubectl get svc
cd /home/akilan/kube-test/
ls
mkdir git-kube-addons
cd git-kube-addons/
ls
git clone https://github.com/akilans/kubernetes.git
cd kubernetes/
ls
ls -la
vi kubernetes-dashboard.yaml 
vi heapster-deployment.yaml 
cat heapster-service.yaml 
kubectl create -f heapster-deployment.yaml 
kubectl create -f heapster-service.yaml 
docker ps
vi influxdb-service.yaml 
vi influxdb-deployment.yaml 
kubectl create -f influxdb-deployment.yaml 
kubectl create -f influxdb-service.yaml 
ls 
mv grafana-deployment grafana-deployment.yaml
vi grafana-deployment.yaml 
vi grafanna-service.yaml 
vi grafana-deployment.yaml 
kubectl get svc --namespace=kube-system
vi grafana-deployment.yaml 
kubectl create -f grafana-deployment.yaml 
kubectl create -f grafanna-service.yaml 
kubectl get svc --namespace=kube-system
docker ps -a
vi heapster-deployment.yaml 
kubectl get svc --namespace=kube-system
vi heapster-deployment.yaml 
kubectl create -f heapster-deployment.yaml 
kubectl delete deployment heapster --namespace=kube-system
kubectl create -f heapster-deployment.yaml 
docker ps -a
docker ps
docker ps -a
kubectl get svc --namespace=kube-system
kubectl get pods --namespace=kube-system
vi grafana-deployment.yaml
kubectl logs pod monitoring-influxdb-1271409385-8watj
kubectl logs pod monitoring-influxdb-1271409385-8watj --namespace=kube-system
kubectl logs pods monitoring-influxdb-1271409385-8watj --namespace=kube-system
kubectl logs --help
kubectl logs monitoring-grafana-387193172-ueq1t
kubectl logs pod  monitoring-grafana-387193172-ueq1t --namespace=kube-system
kubectl get pods --namespace=kube-system
kubectl logs monitoring-grafana-387193172-ueq1t 
kubectl logs monitoring-grafana-387193172-ueq1t --namespace=kube-system
kubectl get pods --namespace=kube-system
kubectl delete svc monitoring-influxdb --namespace=kube-system
kubectl delete deployment monitoring-influxdb --namespace=kube-system
vi influxdb-deployment.yaml
kubectl create -f influxdb-deployment.yaml
docker ps -a
kubectl get pods --all-namespaces
kubectl describe pod monitoring-influxdb-1271409385 --namespace=kube-system
kubectl delete deployment monitoring-influxdb --namespace=kube-system
kubectl get pods --all-namespaces
vi influxdb-deployment.yaml
kubectl create -f influxdb-deployment.yaml
kubectl get pods --all-namespaces
kubectl create -f influxdb-service.yaml
kubectl delete deployment monitoring-grafana --namespace=kube-system
kubectl delete service monitoring-grafana --namespace=kube-system
kubectl delete deployment monitoring-grafana --namespace=kube-system
clear
vi grafana-deployment.yaml
kubectl get svc --namespace=kube-system
vi grafana-deployment.yaml
kubectl create -f grafana-deployment.yaml
ls
kubectl create -f grafanna-service.yaml 
kubectl get pods --all-namespaces
clear
ls
clear
kubectl cluster-info
clear
kubectl cluster-info
curl http://localhost:8080
curl http://localhost:8080/ui
curl http://localhost:8080/ui/
curl http://localhost:8080/api/v1/proxy/namespaces/kube-system/services/kubernetes-dashboard
curl http://localhost:8080/api/v1/proxy/namespaces/kube-system/services/kubernetes-dashboard/
clear
dodcker ps -a
docker ps -a
docker exec -it 409 /bin/bash
docker exec -it 409 /bin/sh
clear
docker ps -a
docker logs 409
cls
clear
docker logs 409
curl http://192.168.3.71:8086/
clear
docker ps -a
kubectl get nodes
docker ps -a
