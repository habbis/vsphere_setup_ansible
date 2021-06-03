# vsphere_setup
vsphere setup habbfarm 


I you want to encrypt variables

To encrypt variables
```
ansible-vault encrypt defaults/main.yml
```

To edit file 
```
ansible-vault edit defaults/main.yml

```
To run playbook with vault
```
ansible-playbook site.yml --ask-vault-pass
```

roles that are tested and are in use

- [esxi_setup](roles/esxi_setup/tasks/main.yml)
- [cluster_setup](roles/cluster_setup/tasks/main.yml)
- [dvswitch_setup](roles/dvswitch_setup/tasks/main.yml)
- [dvswitch_portgroup](roles/dvswitch_portgroup/tasks/main.yml)

roles that are added but not tested or in use

- [resource_pool_setup](roles/resource_pool_setup/tasks/main.yml)
- [vm_vswitch_migration](roles/vm_vswitch_migration/tasks/main.yml)
- [vmk_migration](roles/vmk_migration/tasks/main.yml)
