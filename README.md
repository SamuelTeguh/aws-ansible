[![](https://img.shields.io/badge/SISTECH-LAB-orange.svg)](http://cs.uph.edu)


aws-ansible

This folder provides an example to create aws ec2 instances using Ansible.
In order to get several information such as credential and VM images, you can access several sites as follow:

AMI images:

https://ap-southeast-1.console.aws.amazon.com/ec2/v2/home?region=ap-southeast-1#Images:visibility=public-images;search=ubuntu;sort=name

VPC:

https://ap-southeast-1.console.aws.amazon.com/ec2/v2/home?region=ap-southeast-1#

Access Key and Secret Key:

https://console.aws.amazon.com/iam/home?region=ap-southeast-1#/security_credential

Create key-pair [for example: id_ansible]:

ssh-keygen -t rsa -f ~/.ssh/id_ansible

export /home/your_user_name/.ssh/id_ansible.pub --> to aws

Such as at this site: https://ap-southeast-1.console.aws.amazon.com/ec2/v2/home?region=ap-southeast-1#KeyPairs:sort=keyName

Execute ansible:

ansible-playbook -i hosts ans-aws.yml
