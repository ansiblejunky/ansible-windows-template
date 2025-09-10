# Ansible Windows Automation

Template repository to help kickstart windows automation using Ansible.

```shell
# Install python dependencies
pip install -r requirements.txt
# Install collection dependencies
ansible-galaxy collection install -r collections/requirements.yml
# Install system package dependencies
sudo dnf install $(cat bindep.txt)

# Edit inventory file and ensure variables; domain has to be uppercase
vi hosts/inventory

# Test playbook
ansible-playbook -i hosts/inventory playbooks/example.yml

```