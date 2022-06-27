# Automate Instance on AWS using AWX

## Tasks
1. Create AWS cloud user and secuirty keypair
2. update variables.
   ec2_region - region machine will be deployed
   ec2_instance_type - Machine Type - 
   ec2_image - Define specific OS Amazon image
   ec2_keypair - Secuirty keypair of server login
   ec2_volume_size - Size if server disk
   ec2_count - Number of servers needed
   ec2_security_group_id - firewall config
   ec2_subnet_id - subnet information
   ec2_tag_Role - Tag role fr referencing.
3. Configure this playbook in AWX console.
4. Execute the playbook
5. verify server build status on AWS console or by ssh using the .pem key from AWX host cli.
