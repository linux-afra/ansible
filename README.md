# ansible
This is the playbooks for provisioning some functionality .
#ON NEW Client System
1-adduser ansible .
2-echo "ansible ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers .

#ON Ansible Server
1-su - ansible .
2-ssh-copy-id <Client IP> .

3-echo "[SectionName]" >> /etc/ansible/hosts .
4-echo "<Client IP>" >> /etc/ansible/hosts .
5-ansible-playbook install_<>.yml .

