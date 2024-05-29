Automated Docker Deployment with Ansible on Fedora CoreOS 
Overview
This project aims to automate the deployment of Docker containers using Ansible on a Fedora CoreOS environment. By leveraging Ansible playbooks, we streamline the process of deploying and managing Docker containers, enhancing efficiency and reproducibility.

Prerequisites
Before getting started, ensure the following prerequisites are met:

Fedora CoreOS VM with Docker installed
Ansible installed on the control machine
Access to GitHub repositories for version control (optional)
Usage
1. Clone the Repository
Clone this repository to your local machine:

bash
Copy code
git clone https://github.com/yourusername/ansible-docker-deployment.git
2. Configure Inventory
Edit the hosts.ini file to specify the target hosts for deployment. For example:

ini
Copy code
[local]
localhost ansible_connection=local
3. Customize Playbook (Optional)
Modify the deploy-docker.yml playbook to suit your deployment requirements. You can adjust tasks such as Docker image selection, container names, ports, etc.

4. Execute the Playbook
Run the Ansible playbook to deploy Docker containers:

bash
Copy code
ansible-playbook -i hosts.ini deploy-docker.yml
5. Verification
Verify that the Docker containers are running successfully:

bash
Copy code
docker ps



# 1: Install Ansible on your local machine if you haven't already:

sudo apt-add-repository ppa:ansible/ansible
sudo apt update
sudo apt install ansible

# 2: Clone your code to your local machine

git clone https://github.com/kamranali111/ansible-docker-deployment


# 3: Set up  Ansible inventory file (hosts). 

Replace 192.168.1.100 with the IP address of your Fedora CoreOS VM and ~/.ssh/id_rsa with the path to your SSH private key replace core with the appropriate username in your hosts.ini file. 

# 4: Run the Ansible playbook from your local machine:

ansible-playbook -i hosts.ini deploy-docker.yml


