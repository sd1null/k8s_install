# Ansible playbooks to install k8s

***If you need to choose a version***  

`ansible-playbook ./k8s_install.yml -e target_hosts=hostname -e role=k8s_install_version -e version=1.23.4`

***To install the latest version***
`ansible-playbook ./k8s_install.yml -e target_hosts=hostname -e role=k8s_install_latest`

***Initialization***
`kubeadm init --pod-network-cidr=172.16.0.0/12 --upload-certs --v=5 --kubernetes-version=1.23.4 --control-plane-endpoint=hostname:6443`

