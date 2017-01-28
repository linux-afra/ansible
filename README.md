# ansible
This is the playbooks for provisioning some functionality .
#ON NEW Client System
adduser ansible
echo "ansible ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

#ON Ansible Server
su - ansible \n
ssh-copy-id <Client IP> \n

echo "[SectionName]" >> /etc/ansible/hosts \n
echo "<Client IP>" >> /etc/ansible/hosts \n
ansible-playbook install_<>.yml \n

