# Ansible Deployment Playbooks
Simple Deployment playbooks just to test configuration and Ansible modules.

## Steps:
- Set Hosts Inventory and groups if needed and set vars in it.
```shell
cd ./inventories
vi <lang>_inventory

------
[your_server_group]
ip1
ip2
ip3

[your_server_group:vars]
var=val
var2=val
...

```

Run the playbook:
```shell
ansisble-playbook -i inventories/<lang>_inventory <lang>-deploy.yml
```