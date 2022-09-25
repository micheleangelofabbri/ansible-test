Using a host file instead of the `/etc/ansible/hosts` file, list entries in the given host file
```bash
ansible-inventory \
--inventory hosts.yml \
--list
```

Using ansible-pull, repo should have a local.yml file that will immediately be run
```bash
sudo ansible-pull \
--only-if-changed \
--url https://github.com/micheleangelofabbri/ansible-test.git
```
---
Ansible documentation:
- General:
  - https://docs.ansible.com/ansible/latest/cli/ansible-pull.html
- Modules:
  - https://docs.ansible.com/ansible/latest/collections/ansible/builtin/file_module.html
  - https://docs.ansible.com/ansible/latest/collections/ansible/builtin/apt_module.html
  - https://docs.ansible.com/ansible/latest/collections/ansible/builtin/user_module.html
  - https://docs.ansible.com/ansible/latest/collections/ansible/posix/mount_module.html
