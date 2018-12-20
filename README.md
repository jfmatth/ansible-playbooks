# Playbooks for Linux VPS

Build a VPS and update hosts.ini, then run playbooks below


## bootstrap.yml - Initial VPS bootstrap playbook after VM is built on VPS hosting

```
ansible-playbook bootstrap.yml --ask-pass
```

## patch.yml - Update server and setup 

```
ansible-playbook patch.yml
```
