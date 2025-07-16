# Apigee X Deployment - Jira Story Breakdown

|   Sprint | Story Title                                                            |   Estimation (Story Points) | Epic                                    |
|---------:|:-----------------------------------------------------------------------|----------------------------:|:----------------------------------------|
|        1 | Design Platform-based Terraform module                                 |                           5 | EPIC I - Management Plane and Gateway   |
|        1 | Automate GCP project creation with naming convention                   |                           3 | EPIC I - Management Plane and Gateway   |
|        1 | Enable required GCP APIs for Apigee Deployment                         |                           2 | EPIC I - Management Plane and Gateway   |
|        2 | Implement Apigee X Instance provisioning                               |                           5 | EPIC I - Management Plane and Gateway   |
|        2 | Create Apigee runtime and control plane service accounts               |                           3 | EPIC I - Management Plane and Gateway   |
|        2 | Assign IAM roles for Apigee and networking to respective SAs           |                           2 | EPIC I - Management Plane and Gateway   |
|        3 | Add environment and environment group creation to platform module      |                           5 | EPIC I - Management Plane and Gateway   |
|        3 | Create VPC and Subnet for Apigee X                                     |                           3 | EPIC I - Management Plane and Gateway   |
|        3 | Setup Private Service Connect (PSC) for Apigee runtime                 |                           3 | EPIC I - Management Plane and Gateway   |
|        4 | Validate firewall rules for network components                         |                           2 | EPIC I - Management Plane and Gateway   |
|        4 | Provision Apigee instance in EngLab                                    |                           3 | EPIC I - Management Plane and Gateway   |
|        4 | Create Apigee environments for EngLab and Test                         |                           3 | EPIC I - Management Plane and Gateway   |
|        4 | API Product and Developer app creation blocks                          |                           3 | EPIC I - Management Plane and Gateway   |
|        5 | Provision ILB for Apigee Service Exposure                              |                           3 | EPIC II - ILB & Certificate Integration |
|        5 | Reserve Static Internal IP for Apigee ILB                              |                           1 | EPIC II - ILB & Certificate Integration |
|        5 | Configure backend service and health checks for ILB                    |                           3 | EPIC II - ILB & Certificate Integration |
|        5 | Create certificate for ILB endpoint                                    |                           2 | EPIC II - ILB & Certificate Integration |
|        6 | Upload certificate to Apigee Environment keystore                      |                           2 | EPIC II - ILB & Certificate Integration |
|        6 | Create Truststore in Apigee with backend root/intermediate certs       |                           2 | EPIC II - ILB & Certificate Integration |
|        6 | Link keystore to Apigee Virtual Host                                   |                           2 | EPIC II - ILB & Certificate Integration |
|        6 | Configure Apigee Virtual Host for TLS and bind it to environment group |                           3 | EPIC II - ILB & Certificate Integration |
|        6 | Validate Virtual Host routing with TLS Enabled                         |                           2 | EPIC II - ILB & Certificate Integration |
|        6 | Add Terraform outputs for TLS VHost and Environment group              |                           1 | EPIC II - ILB & Certificate Integration |
|        6 | Create GitHub workflow for deployment                                  |                           3 | Cross-cutting                           |
|        6 | Configure remote backend for state and locking                         |                           2 | Cross-cutting                           |
|        6 | Run Curl test proxy to validate routing from Apigee                    |                           2 | Cross-cutting                           |