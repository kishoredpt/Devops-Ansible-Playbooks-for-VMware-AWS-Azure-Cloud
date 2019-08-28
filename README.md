# DevOps - Ansible Playbooks to Create and Decommission servers in (VMware, AWS, AZURE) and Create a Two-Tierr-Application in AWS.

1. Ansible Playbooks to Provision and Decommission Servers in the VMWare Environment 
2. Ansible Playbooks to Create and Terminate Resources (Servers) in Azure Cloud 
3. Ansible Playbooks to Create and Terminate  EC2 instances in AWS     
4. Ansible playbook to launch Two Tier Server Deployment in AWS 
  --> Ansible Playbook to Create VPC in AWS
  --> Ansible Playbook to Create Public subnet with Internet gateway for Application Server in AWS
  --> Ansible Playbook to Create Private subnet for Database Server in AWS
  --> Ansible Playbook to Create Routetable for Application Server in AWS
  --> Ansible Playbook to Create Application Server (EC2) instance by uisng VPC-Application server subnet(Public subnet) in AWS
  --> Ansible Playbook to Create Database Server (EC2) instance by using VPC-database server subnet (private subnet) in AWS
  --> Ansible Playbook to Create Bastion host (EC2) instance by using public subnet id  in AWS 

executing the two-tier application playbook by using the below commnad

ansible-playbook vpc.yml --extra-vars "vpc_name=test-name" -vvv

5. aws-ec2-deletion.yml --> Playbook Execution for the playbook to delete multiple Ec2 Instances at a time

ansible-playbook aws-ec2-deletion.yml --extra-vars='{"instance_ids": [i-xxxxx,i-xxxx,i-xxxx]}' -vvv
