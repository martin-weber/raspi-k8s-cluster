# raspi-k8s-cluster
Basic setup for a 6+1 node Raspberry Pi 2 Kubernetes Cluster

I followed the instructions on
https://medium.com/nycdev/k8s-on-pi-9cc14843d43
which are based on https://github.com/teamserverless/k8s-on-raspbian/blob/master/GUIDE.md
and put the first part into an ansible-playbook.

Use the following commands to run the playbooks:

Perparation:
```
ansible-playbook -i hosts -u pi --ask-pass prep_k8s_nodes.yml
```

Restart:
```
ansible-playbook -i hosts -u pi --ask-pass restart_nodes.yml 
```

Restart:
```
ansible-playbook -i hosts -u pi --ask-pass shutdown_nodes.yml 
```
