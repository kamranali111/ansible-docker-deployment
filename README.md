
**Automated Docker Deployment with Ansible on Fedora CoreOS**

**Overview**

This project aims to automate the deployment of Docker containers using Ansible on a Fedora CoreOS environment. By leveraging Ansible playbooks, we streamline the process of deploying and managing Docker containers, enhancing efficiency and reproducibility.

**Prerequisites**
Before getting started, ensure the following prerequisites are met:

* Fedora CoreOS VM with Docker installed
* Ansible installed on the control machine (Master)

**Installing Ansible**
If Ansible is not installed on your local machine, follow these steps:

sudo apt-add-repository ppa:ansible/ansible
sudo apt update
sudo apt install ansible


**Cloning the Repository**

Clone this repository to your local machine:

git clone https://github.com/yourusername/ansible-docker-deployment.git

**Configuring Inventory**
Edit the hosts.ini file to specify the target hosts for deployment.

**Customizing Playbook**
Modify the deploy-docker.yml playbook to suit your deployment requirements. You can adjust tasks such as Docker image selection, container names, ports, etc.

**Execution**
Run the Ansible playbook to deploy Docker containers:

ansible-playbook -i hosts.ini deploy-docker.yml

**Verification**
Verify that the Docker containers are running successfully:

docker ps
