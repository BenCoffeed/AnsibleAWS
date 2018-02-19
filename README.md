Read my [blog
post](http://ben.tennant.family/posts/aws-provisioning-with-ansible)
about this project.
# Provisioning AWS resources using Ansible

## Pre-requisites:
- [Ansible](http://docs.ansible.com/ansible/latest/intro_installation.html)
- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/installing.html)

## Usage
Use the provision_resources.yml playbook to build AWS resources in yaml
dictionaries.
`ansible-playbook provision_resources.yml --extra_vars
"inventory=aws_config/ec2/awx01"`

