# Collection of sample ansible roles created during testing

To call the main.yaml in roles, you will have to define a playbook.yaml within roles dir.

sample of playbook.yaml

```
---
- hosts: all
  become: true  #if the action required sudo
  roles:
  - your_roles_name  #/roles/your_roles_name/tasks/main.yaml

