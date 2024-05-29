# 1: Install Ansible on your local machine if you haven't already:

sudo apt update
sudo apt install ansible -y

# 2: Clone your code to your local machine

git clone https://github.com/kamranali111/ansible-docker-deployment


# 3: Set up  Ansible inventory file (hosts). 

Replace 192.168.1.100 with the IP address of your Fedora CoreOS VM and ~/.ssh/id_rsa with the path to your SSH private key in your hosts.ini file.

# 4: Run the Ansible playbook from your local machine:

ansible-playbook -i hosts.ini deploy-docker.yml
