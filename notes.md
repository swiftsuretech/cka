network policy 
  - namespaces
  - pods in certain namespace can only communicate to other namespace 
  - port restricted
  - restrict to those that DO have port open

pods:
  - Schedule on node based on label

broken node:
  - Fix a node with kubelet broken
  - Make fix permanent

networking:
  - Expose a service nginx with a named port (80)
  - Add additional NodePort

maintenance:
  - Cordon and drain a node
  - Schedule a pod to test


etcd snapshot:
  - Referred to a 127.0.0.1 address only rather than node


sidecar Container:
  - Add sidecar to pod that runs logging command
  - Mount a shared vol with existing pod
  - Check output of sender from original pod


Loadbalancer deployment:
  - Scale up with record flag


upgrade:
  - control plane only from 1.24.1 to 1.24.2
  - cordon and drain
  - upgrade kubeadm
  - upgrade kubelet and kubectl
  - uncordon node


RBAC:
  - create service account
  - create a cluster role to create 3 types of object
  - create corresponding CRB for specific namespaces


kubectl Tasks (1):
  - count number of nodes without NoSchedule taint

kubectl Tasks (2):
  - get logs from a pod / apply grep and save

kubectl Tasks (3):
  - find node using most CPU based on label