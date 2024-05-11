This GitLab CI/CD configuration defines three stages:

--> lint: Checks Terraform code formatting (terraform fmt), validates the Terraform configuration (terraform validate), and performs static analysis (tflint).

--> plan: Initializes Terraform (terraform init) and generates an execution plan (terraform plan) to preview changes.

--> apply: Applies the Terraform changes (terraform apply) using the plan generated in the previous stage. This stage is triggered only for changes pushed to the master branch.
