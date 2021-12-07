# Ansible playbook for setup Kubernetes Cluster

This repo is used for deployment of Kubernetes cluster (kubeadm) with docker and flannel. Tested on EC2 instances, Ubuntu 20.04

You can run separately roles for creating users, setting up dependencies or joining worker nodes. Change IP to your nodes in ```hosts``` file.

**Example:
```
ansible-playbook kube-dependencies.yml -i hosts --private-key="ubuntu.pem" --extra-vars="user=ubuntu" -v
```

