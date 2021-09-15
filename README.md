# Ansible-webapp
- Simple web app deployment through Ansible and a docker container

# Check your file syntax 
- Install ansible lint

- sudo yum install python-pip
- sudo pip install ansible-lint
- ansible-lint deploy.yml

# Run the playbook

- ansible-playbook -i hosts.yml deploy.yml

# Ansible verbose option

- ansible-playbook -i hosts.yml -vvv deploy.yml

# Ansible vault and security commands

 Encrypt file
- ansible-vault encrypt files/secrets/credentials.yml

 Decrypt file
- ansible-vault decrypt files/secrets/credentials.yml

- Run playbook with vault encrypted
ansible-playbook -i hosts.yml --ask-vault-pass deploy.yml
