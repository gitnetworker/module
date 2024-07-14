Simple project

    S3 Module: The module in module/s3 defines the creation of an S3 bucket with variable inputs for the bucket name and tags.
    
    Main Terraform Script: The main script (main.tf in the base folder) uses this module to create three different S3 buckets with distinct names and tags, based on the environment type (dev or prod) specified in the variable files (dev-terraform.tfvars and prod-terraform.tfvars).
    
    Provider Configuration: The providers.tf file sets up the AWS provider to use the us-east-1 region.
    
    Environment Variables: The environment type variable is defined in variables.tf and is populated by the respective .tfvars files for different environments.
    
    This setup allows for reusable, modular, and environment-specific S3 bucket configurations in AWS using Terraform.
