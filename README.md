# ansible_vmware_deploy_provision
Use Ansible to deploy VMware template, add to dynamic inventory and provision.

Deploy
```
# ansible-playbook deploy.yml
```
Destory
```
# ansible-playbook destroy.yml
```

Example Spec sheet
```
spec:
  nodes:
  - name: justai-web01
    os: Centos7
    services:
    - nginx
    - motd
    ip: 192.168.30.111
    netmask: 255.255.255.0
    gateway: 192.168.30.1
    disk_size: 50
    mem: 1024
  - name: justai-db01
    os: Centos7
    services:
    - mysql
    - motd
    ip: 192.168.30.112
    netmask: 255.255.255.0
    gateway: 192.168.30.1
    disk_size: 50
```
