# My Ansible Playbooks

List:
  - lamp: A Playbook to Install LAMP on Fedora 29. Uses DNF package manager and python3. 
    - Requires: ansible_python_interpreter=/usr/bin/python3 in hosts.inv file
    - Grant Public Key Authentication: ssh-copy-id -i /home/han/.ssh/id_rsa_ansible.pub r2d2@aa-589
    - Running: ansible-playbook -i ./hosts.inv -u r2d2 -K ./playbook.yml
    - Testing: lynx http://aa-589/db.php; lynx http://aa-589/index.php
    - Description: Using Fedora release 29 as control workstation, and the same for target systems.
      - Running target systems in Gnome Boxes for testing
      - Using Ansible installed from dnf repository: sudo dnf install ansbile
