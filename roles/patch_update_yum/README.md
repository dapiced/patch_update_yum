# Ansible Role: patch_update_yum

An Ansible role that upgrade all packages or security patch only via yum and reboot server (optional) 

# Description 

This playbook allows you to apply patch update via yum
4 types of update available: everything with or without reboot OR security only with or without reboot
The hosts must be a part of the patch_update_yum group if desired
You must configure the variables "securite_only" (yes or no) and "reboot" (yes or no) in the group_vars "patch_update_yum" or default wil be all patch with reboot
You need ansible 2.7 to use the reboot module



