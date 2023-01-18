# zabbix-agent-dev



## Requirement 

```
# RHEL/Oracle
yum install ansible
# Debian/Ubuntu
apt install ansible
```

## Edit Host/Inventory File

If using private key:

```
[all:vars]
ansible_connection=ssh
ansible_user=root
ansible_ssh_private_key_file=~/.ssh/id_rsa

[webserver]
example.com
server.com

[database]
192.168.1.1
```


If using user and password

```
[all:vars]
ansible_connection=ssh
#ansible_user=root
#ansible_ssh_private_key_file=~/.ssh/id_rsa

[webserver]
example.com

[webserver:vars
ansible_user=root
ansible_ssh_pass=gEd$s7SWL#8idG
ansible_sudo_pass=gEd$s7SWL#8idG

```

