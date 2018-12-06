### 1. 環境の準備

```
# get source ansible playbook
git clone https://github.com/phongnx1/ansible-docker-training.git
# get application
# cd ansible-playbook
# git clone

# start VMs
vagrant up ci consumer

# install for ci and consumer
vagrant ssh ci
cd ansible-playbook
ansible-playbook -i hosts.local provision.yml --become

# install mysql by docker-compser
ansible-playbook -i hosts.local install_mysql.yml--become
```
