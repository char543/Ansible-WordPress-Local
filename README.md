# Ansible-WordPress-Local
Ansible playbook to deploy wordpress on Ubuntu for local development.

I didn't want this to be complex or out of reach to anyone not familiar with ansible so i wanted to keep this playbook in a single file and as user friendly as possible.

For now it is tested on ubuntu 18.04 but may work on other variants.

## What does it do?
One click deploy latest WordPress package on Ubuntu for a local development environment.

### Steps
You may want to change the variables at the top of the playbook but for local deployment/testing purposes these should be ok.

vars: username: nonroot ***# (name of non root user for server setup and operation)***  
mysql_user: dbuser ***# (name of database user)***  
mysql_pass: pass ***# (mysql user password)***  
mysql_db: wpdb ***# (wordpress database name)***  
mysql_root_pass: root ***# (mysql root password)***  
email: your-email@site.com ***# (your email address)***  
domain: yourdomain.com ***# (your site domain)***  

#### 1) Install Ansible with this command
`sudo apt update && sudo apt install software-properties-common && sudo apt install python-apt -y && sudo apt-add-repository --yes --update ppa:ansible/ansible && sudo apt install ansible -y`

#### 2) Run playbook
`sudo ansible-playbook local-site.yml`
