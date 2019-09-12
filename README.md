Install k3s
```bash
ansible-playbook -i inventory k3s.yml 
```

Uninstall k3s
```bash
ansible-playbook -i inventory k3s_uninstall.yml 
```

Shutdown all nodes and masters
```bash
ansible all -i inventory --become -a halt
```