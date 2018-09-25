

## Playbook to create a new VM in Ovirt

## Requirements

The below requirements are needed on the host that executes this playbook.

1. Ansible >= 2.3
2. python >= 2.7
3. ovirt-engine-sdk-python >= 4.2.4


## To Create a new VM Follow below steps:

 Copy the file vars.yml located in vars directory and fill below variables:

   1. ovirt_url :
   2. ovirt_username
   3. ovirt_password
   4. ca_certificate  
   5. vm_name : Name of VM to be created
   6. vm_memory : Physical Memory to be allocated
   7. vm_cpu_cores: VCpu cores to be allocated to VM
   8. vm_hdd_size: Size of Drive in Gibs to be attached to VM
   9. vm_network : Name of VLan VM should be attached
  10. vm_network_profile: Profile of VLAN 

 Run the playbook using below command
   $ ansible-playbook main.yml

## Note:

If you do not have ca certificate downloaded on the host, follow the first point in the document
 https://docs.google.com/document/d/1VwpDzDIHAFlrvl7zSnk3MnM5wP3qt3pX-M-1pVZT9fs/edit?usp=sharing  

Please refer sample file  vars/DJ_api_vars.yml.

If you have to create multiple VMs at at time, make copies of  vars.yml file and edit them. Run the  main playbook by including the new var file in playbook one at a time.

