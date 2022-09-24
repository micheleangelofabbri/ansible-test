List entries in the given host file
```bash
ansible-inventory \
--inventory hosts.yml \
--list
```

Run ansible playbooks locally
```bash
ansible-playbook \
--inventory hosts.yml \
--connection=local \
ls_playbook.yml
```