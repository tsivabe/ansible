# Automate Instance and Apache Server on GCP using AWX

## Prerequisites
1. Create [Project](https://console.cloud.google.com/projectselector/compute/instances) on Google Cloud Platform. 
2. Create a [Serviceaccount](https://console.cloud.google.com/iam-admin/serviceaccounts) with editor access. (Refer [Creating-service-account](https://cloud.google.com/compute/docs/access/create-enable-service-accounts-for-instances))
3. Download [.JSON credentials file](https://support.google.com/cloud/answer/6158849?hl=en&ref_topic=6262490#serviceaccounts) of created service account.
4. Edit instance_name in [vars/main.yml](vars/main.yml), by default it is centos-7.
5. Edit machine_type in [vars/main.yml](vars/main.yml), by default it is e2-micro.
6. Edit zone in [vars/main.yml](vars/main.yml), by default it is us-central1-a.
7. Edit source_image in [vars/main.yml](vars/main.yml), by default it is CENTOS-7.
8. Give project id, .JSON file_path in [vars/main.yml](vars/main.yml) file. 
9. Execute the Job from AWX console once the Job completes.
10. Your Google Compute Engine Instance is now created, with Apache Server installed in it.
11. Browse to instance public ip address.
