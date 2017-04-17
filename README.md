# ansible_aws_opencms

Run the following commands to launch instance and configure ec2 instances

Set the following environment variables

export AWS_ACCESS_KEY_ID=" "
export AWS_SECRET_ACCESS_KEY=""

=Create Instance :

	Command : ansible-playbook opencms/site.yml

Configure and install web,app and db

	Commands: ansible-playbook -i hosts mysql.yml
		  ansible-playbook -i hosts apache.yml
		  ansible-playbook -i hosts tomcat.yml

