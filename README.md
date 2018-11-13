# devops-cloudformation-wordpress
Cloudformation example to launch simple wordpress instance with a local mysql database.

Execute cloudformation stack using AWS CLI to launch VPC infrastructure and launch EC2 instance to host wordpress

Contents:
1) wordpress.template : High level nested template with references to vpc creation and EC2 instance creation template
2) vpc_creation.template:  Template that creates VPC, public and private subnets, IG, NAT gateways and default routes
3) ec2_instance.template: Template that creates a wordpress instance on Centos AMI. 
