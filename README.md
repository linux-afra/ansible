# ansible
This is the playbooks for provisioning some functionality .
#ON NEW Client System
adduser ansible
echo "ansible ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

#ON Ansible Server
su - ansible
ssh-copy-id <Client IP>

echo "[SectionName]" >> /etc/ansible/hosts
echo "<Client IP>" >> /etc/ansible/hosts
ansible-playbook install_<>.yml

