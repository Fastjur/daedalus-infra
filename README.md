# daedalus-infra

## Ansible
Follow installation instructions from ansible: https://docs.ansible.com/ansible/latest/index.html

Then, to update the inventory, run:
```
ansible-playbook daedalus.yaml -i inventory.yaml -K
```

Note: the `-K` flag is required to run the playbook as root, this will prompt for the root password.