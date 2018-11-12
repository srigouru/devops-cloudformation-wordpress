# devops-cloudformation-wordpress
Cloudformation example to launch simple wordpress instance with a local mysql database.

Execute cloudformation stack to launch VPC infrastructure and launch EC2 instance to host wordpress

>> aws cloudformation create-stack --stack-name wordpress-candidate-oouj5bu082 --template-url https://s3.amazonaws.com/candidate-oouj5bu082/wordpress.template

1) wordpress.template : High level nested template with references to vpc creation and EC2 instance creation template
2) vpc_creation.template:  Template that creates VPC, public and private subnets, IG, NAT gateways and default routes
3) ec2_instance.template: Template that creates a wordpress instance on Centos AMI. 
