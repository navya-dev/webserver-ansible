# Ansible Playbook to Launch Ec2 instance, install httpd webserver and host website.

This is a sample Ansible playbook to create and provision webserver that serves html page.
This is executed using ec2 instance as localhost, with ansible installed on it. 

## Playbook.yml does the following:

> Creates Security Group
> Creates Load Balancer that listens to port 80
> Spinning up an EC2 instance
> Adding this EC2 instance as known host.
> Adding EC2 instance to ELB.
> Installing httpd server
> Creating html page on the webserver.
> Creating and  attaching SSL certificate.
> Routing requests from http to https.

###Prerequisites:

Ansible 2.2
python 2.7
boto3
aws cli

Command to RUN playbook

``` AWS_PROFILE=personal ansible-playbook -i playbook.yml ```


ec2_vars.yml file is provided to add variables that are required.

The above can be done using Cloudformation templates as well if we want to utilize resources provided by AWS.















