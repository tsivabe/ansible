# Automate Hadoop CLuster deploy on AWS using AWX

## EC2 Build Variables
1. Create AWS cloud user and secuirty keypair
2. update variables.
   region_name - region machine will be deployed
   instance_flavour - Machine Type - 
   ami_id - Define specific OS Amazon image
   keypair - Secuirty keypair of server login
   ec2_volume_size - Size if server disk
   ec2_count - Number of servers needed
   sg_name - firewall config
   subnet_name - subnet information
   instance_tag - Tag name to servers


## Kubernetes Master, Slave Variables
   service_names - required packages and services.
   hadoop_folder - folder contains cluster info

3. Configure the kubecluster_deploy.yml  playbook in AWX console.
4. Execute the playbook
5. verify server build status on AWS console or by ssh using the .pem key from AWX host cli.