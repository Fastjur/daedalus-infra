# daedalus-infra

## Ansible
Follow installation instructions from ansible: https://docs.ansible.com/ansible/latest/index.html

Then, to update the inventory, run:
```bash
ansible-playbook daedalus.yml -i inventory.yml -K
```

Note: the `-K` flag is required to run the playbook as root, this will prompt for the root password.

### Testing the playbook
If you first want to dry-run the playbook, run:
```bash
ansible-playbook daedalus.yml -i inventory.yml -K --check --diff
```