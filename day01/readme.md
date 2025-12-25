# Introduction to Terraform

### Terraform helps you create and manage cloud resources using code instead of doing everything manually.

---

## Key Learnings

- Infrastructure setup : Terraform stores infrastructure settings in files so the same environment can be recreated anytime.
- Providers : Providers allow Terraform to connect to cloud platforms like AWS or Azure to create and manage resources.
- Terraform plan : Terraform shows what will change before applying it, which keeps updates safe and predictable.
- Statefile : A state file tracks deployed resources, helping Terraform decide what to add, change or remove.
- Variables and modules : Variables and modules let you reuse configuration and manage different environments more easily.
- Immutable deployments : Terraform replaces resources instead of editing them manually, which keeps deployments consistent.
- Version control : Using Git with Terraform helps track changes, collaborate as a team and roll back when needed.
---

## Common Terraform Commands
- terraform init : Prepares the working directory and downloads required providers.
- terraform plan : Shows what changes will happen before applying them.
- terraform apply : Applies the planned changes and provisions or updates infrastructure.
- terraform fmt : Formats configuration files to keep the code readable and consistent.
- terraform validate : Checks the configuration files to ensure they are valid before running a plan or apply.
- terraform show : Displays details of deployed infrastructure recorded in the state file.
- terraform output : Shows output values defined in the configuration, often used by other tools or teams.
- terraform destroy : Removes all infrastructure created by Terraform when it is no longer needed.

---

## Installing Terraform on Windows

Follow these steps to install Terraform on a Windows system.

### Step 1: Download the binary

1. Open the Terraform install page:  
   https://developer.hashicorp.com/terraform/install
2. Select **Windows**
3. Download the ZIP file for your architecture (usually `amd64`)

### Step 2: Extract the binary

1. Extract the ZIP file
2. Move the `terraform.exe` file to a directory, for example:
C:\terraform

markdown
Copy code

### Step 3: Add Terraform to the PATH

1. Open **Start** and search for **Environment Variables**
2. Select **Edit the system environment variables**
3. Click **Environment Variables**
4. Under **System variables**, select **Path** and click **Edit**
5. Click **New** and add the directory path:
C:\terraform

markdown
Copy code
6. Click **OK** to save

### Step 4: Verify the installation

Open **PowerShell** or **Command Prompt** and run:
terraform -version

yaml
Copy code

A version output confirms successful installation.

---
