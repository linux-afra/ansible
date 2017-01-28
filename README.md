# ansible
This is the playbooks for provisioning some functionality .
#ON NEW Client System
`adduser ansible  <br />
echo "ansible ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers  <br />`

#ON Ansible Server
`su - ansible  <br />
ssh-copy-id <Client IP> <br />  
echo "[SectionName]" >> /etc/ansible/hosts  <br />
echo "<Client IP>" >> /etc/ansible/hosts  <br />
ansible-playbook install_<>.yml  <br />`

