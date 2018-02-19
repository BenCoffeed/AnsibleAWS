Read my [blog
post](http://ben.tennant.family/posts/aws-provisioning-with-ansible-p1)
about this project.
# Provisioning AWS resources using Ansible

## Pre-requisites:
- [Ansible](http://docs.ansible.com/ansible/latest/intro_installation.html)
- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/installing.html)
- [Vault](https://vault.io)
- [Vault AWS Secret Engine](https://www.vaultproject.io/docs/secrets/aws/)

## Usage
Use the provision_resources.yml playbook to build AWS resources in yaml
dictionaries.
`ansible-playbook provision_resources.yml --extra_vars
"inventory=aws_config/ec2/awx01"`

## Setup
This playbook assumes that you have a Vault server running and the AWS
secret engine installed with a policy living at `aws/roles/production_provision_resources:access_key` that has rights to manage EC2 resources.
