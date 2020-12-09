# Instructions 
---
## Install Ansible

`sudo yum install epel-release -y`

`sudo yum install ansible -y`

## Topics covered
1. Day1     
    - Basic inventory file
    - Check connectivity using ping.yml playbook
    - Install Nginx and use of handler
2. Day2
    - Jinja Templates
        - Update the html file in default  nginx folder path 
    - Loops
        - Until
        - loop
        - loop retry
        - loop control
    - Conditions in playbook
        - Install packages based on OS type
        - Multiple condition in when statement
    - Error Handling
        - Purposefully ignore the errors
        - Failed the task based on condtion  
   

## Run playbook

`ansible-playbook -i environments/internal_env/ ping.yml`

## Overwrite the default vars using extra_vars (-e) option
`ansible-playbook -i environments/internal_env/ loops.yml -e "user1=test user2=abcd"`