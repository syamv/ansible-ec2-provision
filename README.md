# ansible-ec2-provision
ansible-ec2-provision


Usage:

Create a variables file using ec2_vars/sample.yml as a template.

E.g.

cp ec2_vars/sample.yml ec2_vars/webservers.yml
vi ec2_vars/webservers.yml

After setting all variables, run it:

ansible-playbook -vv -i /etc/ansible/ec2.py -e "type=webservers" provision-ec2.yml
