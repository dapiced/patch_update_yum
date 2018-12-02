
This playbook allows to apply an update of RHEL patch via yum
==============================================================

- By default, it updates all the patches and restart the server

- 6 types of update are available

      - All patches with restart
      
      - All patches without restart
      
      - Security patch only with restart
      
      - Security patch only without restart
      
      - Custom patch only with restart
      
      - Custom patch only without restart
      

- The following variables must be overwritten only if the default does not suit your need (eg by a group_vars patch_update)

      - security_only_required: "no" # yes/no
   
      - reboot_required: "true"      # true/false
   
      - package_name: '*'            # yum package name
   
      - package_state: "latest"      # absent, installed, latest, present, removed
    
- You need ansible 2.7 to use the reboot module



