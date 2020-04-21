# Ansible-WordPress-Local
Ansible playbook to deploy wordpress on Ubuntu for local development.

I didn't want this to be complex or out of reach to anyone not familiar with ansible so i wanted to keep this playbook in a single file and as 'one liner' as possible.

For now it is tested on ubuntu 18.04 but may work on other variants.

## What does it do?
One click deploy latest WordPress package on Ubuntu for a local development environment.

### Steps

#### 1) Install Ansible with this command
sudo apt update && sudo apt install software-properties-common && sudo apt install python-apt -y && sudo apt-add-repository --yes --update ppa:ansible/ansible && sudo apt install ansible -y

#### 2) Run playbook
sudo ansible-playbook local-site.yml
