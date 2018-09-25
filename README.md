

Playbook to create a new VM in Ovirt

Setup

The below requirements are needed on the host that executes this playbook.

1. Ansible >= 2.3
2. python >= 2.7
3. ovirt-engine-sdk-python >= 4.2.4


Create a new VM

 Edit the file vars.yml in vars directory and fill below variables:

   1. ovirt_url 
   2. ovirt_username
   3. ovirt_password
   4. ca_certificate 
   5. vm_name
   6. vm_memory 
   7. vm_cpu_cores
   8. vm_hdd_size
   9. vm_network
  10. vm_network_profile

  
