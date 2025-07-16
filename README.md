quick use

# Apigee X Deployment - Jira Story Breakdown (6 Sprints Plan)

## EPIC I - PTIDE 30842: Management Plane and Gateway

### Sprint 1

**Story 1: Design Platform-based Terraform module**
- Description: Create a Terraform module to support platform-based Apigee deployment instead of core/LOB model.
- Estimation: 5 story points

**Story 2: Automate GCP project creation with naming convention**
- Description: Create a script/module to automate GCP project provisioning based on predefined naming convention.
- Estimation: 3 story points

**Story 3: Enable required GCP APIs for Apigee Deployment**
- Description: Enable GCP APIs like Apigee, Compute Engine, IAM, and Service Networking for Apigee Deployment.
- Estimation: 2 story points

---

### Sprint 2

**Story 4: Implement Apigee X Instance provisioning**
- Description: Deploy Apigee X instance using Terraform in EngLab project.
- Estimation: 5 story points

**Story 5: Create Apigee runtime and control plane service accounts**
- Description: Provision appropriate service accounts with required IAM permissions.
- Estimation: 3 story points

**Story 6: Assign IAM roles for Apigee and networking to respective SAs**
- Description: Assign fine-grained roles to runtime and network service accounts.
- Estimation: 2 story points

---

### Sprint 3

**Story 7: Add environment and environment group creation to platform module**
- Description: Add support for Apigee environment and environment group in Terraform module.
- Estimation: 5 story points

**Story 8: Create VPC and Subnet for Apigee X**
- Description: Define and provision custom VPC and subnets for Apigee X.
- Estimation: 3 story points

**Story 9: Setup Private Service Connect (PSC) for Apigee runtime**
- Description: Configure PSC for private connectivity to Apigee runtime.
- Estimation: 3 story points

---

### Sprint 4

**Story 10: Validate firewall rules for network components**
- Description: Ensure all firewall rules are correctly set for Apigee and backend communication.
- Estimation: 2 story points

**Story 11: Provision Apigee instance in EngLab**
- Description: Final provisioning of Apigee instance using validated network and IAM setup.
- Estimation: 3 story points

**Story 12: Create Apigee environments for EngLab and Test**
- Description: Create and validate environments within the provisioned Apigee instance.
- Estimation: 3 story points

**Story 13: API Product and Developer app creation blocks**
- Description: Add API product and app creation to the Terraform module.
- Estimation: 3 story points

---

## EPIC II - Apigee X Internal Load Balancer & Certificate Integration

### Sprint 5

**Story 14: Provision ILB for Apigee Service Exposure**
- Description: Create an internal load balancer for exposing Apigee runtime to internal clients.
- Estimation: 3 story points

**Story 15: Reserve Static Internal IP for Apigee ILB**
- Description: Allocate internal IP address for the ILB.
- Estimation: 1 story point

**Story 16: Configure backend service and health checks for ILB**
- Description: Define ILB backend service and configure health checks.
- Estimation: 3 story points

**Story 17: Create certificate for ILB endpoint**
- Description: Generate and provision certificate for secure ILB endpoint.
- Estimation: 2 story points

---

### Sprint 6

**Story 18: Upload certificate to Apigee Environment keystore**
- Description: Add certificate to Apigee keystore associated with the environment.
- Estimation: 2 story points

**Story 19: Create Truststore in Apigee with backend root/intermediate certs**
- Description: Add backend CA certificates to Apigee truststore.
- Estimation: 2 story points

**Story 20: Link keystore to Apigee Virtual Host**
- Description: Bind keystore to the virtual host for TLS termination.
- Estimation: 2 story points

**Story 21: Configure Apigee Virtual Host for TLS and bind it to environment group**
- Description: Setup and bind virtual host to environment group with TLS enabled.
- Estimation: 3 story points

**Story 22: Validate Virtual Host routing with TLS Enabled**
- Description: Test and verify routing through TLS-enabled virtual host.
- Estimation: 2 story points

**Story 23: Add Terraform outputs for TLS VHost and Environment group**
- Description: Add final outputs to Terraform for TLS virtual host and env group references.
- Estimation: 1 story point

---

### Cross-cutting (Optional/Parallel Stories)

**Story: Create GitHub workflow for deployment**
- Description: Automate Terraform deployment using GitHub Actions.
- Estimation: 3 story points

**Story: Configure remote backend for state and locking**
- Description: Setup remote state backend (e.g., GCS + state locking).
- Estimation: 2 story points

**Story: Run Curl test proxy to validate routing from Apigee**
- Description: Deploy a test proxy and validate routing end-to-end.
- Estimation: 2 story points
