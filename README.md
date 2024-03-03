"# Infa_Auto_CA1_Ansible" 


1. Configure the EC2 instances in the Ansible hosts file.
- sudo vi /etc/ansible/hosts
[servers]
<IP1> ansible_user=ec2-user ansible_python_interpreter=/usr/bin/python
<IP2> ansible_user=ec2-user ansible_python_interpreter=/usr/bin/python

2. Add the labuser key pair to the SSH agent.
- cd ~ && eval `ssh-agent -s` && vi labuser.pem
- chmod 400 labuser.pem && ssh-add labuser.pem

3. Clone the Git repository.

git clonse https://github.com/PatrickCulligan/Infa_Auto_CA1_Ansible.git
