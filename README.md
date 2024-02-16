# Google Cloud Confidential VM
Deploy a hardened Confidential VM instance with Terraform for running your sensitive workloads on Google Cloud. 
Confidential VMs will encrypt data in-use as an extra layer on top of the by default enabled encryption at rest and in transit. 

**What will be part of the Confidential VM solution?**
1. Deploy Confidential Compute VM
2. Create custom VPC with subnet
3. Disk encryption keys
4. VPC Service Control Perimeter 
5. Organisation Policy Constraint (Block default service account, compute.vmExternalIpAccess, trustedImageProjects)
6. Secure Web Proxy for filtering egress traffic on the Confidential VM
7. Block access to public DNS

**Running the Terraform plan**
Make sure to adjust the Google Cloud project in the variables.tf file before deploying and change the "awesomename" placeholder to something Awesome ;) 
