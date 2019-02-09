# My Ansible Playbooks

List:
  - lamp: a playbook to install LAMP on Fedora (29 so far)
    - Requires: ansible_python_interpreter=/usr/bin/python3 in hosts.inv file
    - ssh-copy-id -i /home/han/.ssh/id_rsa_ansible.pub r2d2@aa-589
    - ansible-playbook -i ./hosts.inv -u r2d2 -K ./playbook.yml
     

