# Ansible playbook for setup Kubernetes Cluster

This repo is used for deployment of Kubernetes cluster (kubeadm) with docker and flannel. Tested on EC2 instances, Ubuntu 20.04

Change IP addresses to IP of your nodes in ```hosts``` file, define ```user``` in ```extra-vars``` block, and run playbook.

**Example:
```
ansible-playbook deploy.yml -i hosts --private-key="ubuntu.pem" --extra-vars="user=ubuntu" -v
```

