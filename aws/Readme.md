✅ Requirements

Ansible >=2.10

amazon.aws collection
Install with:

ansible-galaxy collection install amazon.aws


AWS Credentials:
Store your credentials securely using Ansible Vault or environment variables.

export EC2_ACCESS_KEY=your_access_key
export EC2_SECRET_KEY=your_secret_key

🔐 Using Ansible Vault (Recommended)

You can encrypt your AWS credentials with Ansible Vault:

ansible-vault create group_vars/all/vault.yml


Inside vault.yml:

ec2_access_key: YOUR_ACCESS_KEY
ec2_secret_key: YOUR_SECRET_KEY


Run the playbook with vault password:

ansible-playbook aws-instance.yml --ask-vault-pass

📍 Notes

Make sure your default VPC and security group exist in the selected region.

You can uncomment and modify key_name and vpc_subnet_id as needed for SSH access or custom networking.

This example uses a public Amazon Linux 2 AMI in us-east-1.

🧹 Cleanup (Optional)

Terminate the instance manually or write a teardown playbook to avoid unexpected AWS charges.
