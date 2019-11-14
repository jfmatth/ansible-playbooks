# Playbooks for Linux VPS

Build a VPS and update hosts.ini, then run playbooks below


## bootstrap.yml - Initial VPS bootstrap playbook after VM is built on VPS hosting

```
ansible-playbook bootstrap.yml -k -b (-u if needed)

-k = Ask Password
-b = Become
-u = User
```


## patch.yml - Update server and setup

You must run ssh-agent to load your ssh key into memory
```
eval `ssh-agent`
ssh-add
```

Then run the playbook to patch the server


```
ansible-playbook patch.yml
```
