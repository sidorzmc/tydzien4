
Minikube:

kubectl cluser-info
 $ ./minikube.exe kubectl cluster-info
Kubernetes master is running at https://192.168.99.101:8443
KubeDNS is running at https://192.168.99.101:8443/api/v1/namespaces/kube-system/services/kube-dns:dns/proxy

PS C:\Program Files\Kubernetes\Minikube> kubectl get pods
NAME                          READY   STATUS              RESTARTS   AGE
hello-node-7676b5fb8d-xdkzj   0/1     ContainerCreating   0          7s

PS C:\Program Files\Kubernetes\Minikube> kubectl get pods --all-namespaces
NAMESPACE     NAME                               READY   STATUS    RESTARTS   AGE
kube-system   coredns-5644d7b6d9-mgslq           1/1     Running   2          11d
kube-system   coredns-5644d7b6d9-n9bwn           1/1     Running   2          11d
kube-system   etcd-minikube                      1/1     Running   1          24m
kube-system   kube-addon-manager-minikube        1/1     Running   2          11d
kube-system   kube-apiserver-minikube            1/1     Running   1          24m
kube-system   kube-controller-manager-minikube   1/1     Running   1          24m
kube-system   kube-proxy-tw6z8                   1/1     Running   2          11d
kube-system   kube-scheduler-minikube            1/1     Running   2          11d
kube-system   storage-provisioner                1/1     Running   2          11d


Azure:

$ ./minikube.exe kubectl config get-contexts
CURRENT   NAME       CLUSTER    AUTHINFO                      NAMESPACE
*         AKSlab4    AKSlab4    clusterUser_AKSlab4_AKSlab4
          minikube   minikube   minikube
		  


kubectl cluster-info
Kubernetes master is running at https://akslab4-akslab4-1c88a2-42ca13d0.hcp.westeurope.azmk8s.io:443
healthmodel-replicaset-service is running at https://akslab4-akslab4-1c88a2-42ca13d0.hcp.westeurope.azmk8s.io:443/api/v1/namespaces/kube-system/services/healthmodel-replicaset-service/proxy
CoreDNS is running at https://akslab4-akslab4-1c88a2-42ca13d0.hcp.westeurope.azmk8s.io:443/api/v1/namespaces/kube-system/services/kube-dns:dns/proxy
kubernetes-dashboard is running at https://akslab4-akslab4-1c88a2-42ca13d0.hcp.westeurope.azmk8s.io:443/api/v1/namespaces/kube-system/services/kubernetes-dashboard/proxy
Metrics-server is running at https://akslab4-akslab4-1c88a2-42ca13d0.hcp.westeurope.azmk8s.io:443/api/v1/namespaces/kube-system/services/https:metrics-server:/proxy


kubectl get nodes
NAME                                STATUS   ROLES   AGE   VERSION
aks-nodepool1-19583444-vmss000000   Ready    agent   92m   v1.13.11


kubectl get pods --all-namespaces
NAMESPACE     NAME                                    READY   STATUS    RESTARTS   AGE
kube-system   coredns-866fc6b6c8-25jhx                1/1     Running   0          121m
kube-system   coredns-866fc6b6c8-pgnzj                1/1     Running   0          126m
kube-system   coredns-autoscaler-657d77ffbf-6zvl6     1/1     Running   0          126m
kube-system   kube-proxy-t84gw                        1/1     Running   0          122m
kube-system   kubernetes-dashboard-6f697bd9f5-98hbp   1/1     Running   0          126m
kube-system   metrics-server-58699455bc-hqwg7         1/1     Running   0          126m
kube-system   omsagent-rs-6787c656bc-tjtrp            1/1     Running   0          126m
kube-system   omsagent-t9v8p                          1/1     Running   0          122m
kube-system   tunnelfront-58ffb8d78b-cwv5v            1/1     Running   0          126m
