

Commande d'execution : 

ansible-playbook -i inventory/hosts.ini playbooks/deploy-ssh-pqc.yml

ansible/
   -inventory/
     ├── production.ini
     └── staging.ini
     
 ├  -group_vars/
 │   ├── all.yml
 │   ├── debian.yml
 │   └── redhat.yml
 
 ├─- playbooks/
 │   ├── site.yml
 │   ├── webservers.yml
 │   └── hardening.yml
 
 └── roles/
     ├── nginx/
     │   ├── tasks/
     │   │   └── main.yml
     │   ├── handlers/
     │   │   └── main.yml
     │   ├── templates/
     │   └── defaults/
     │       └── main.yml
     
     └── users/
         ├── tasks/
         │   └── main.yml
         └── defaults/
         
             └── main.yml
