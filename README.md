#Terraform
- used to build/manage infrastructure

As part of this spike, I have made the use of terraform to add resources for aws to add a ec2 instace and azure to add a dns record

#Running terraform with CLI

### AWS - Adding a simple ec2 instance
Before running terraform with the CLI, you will need to make sure that out have set up your aws credentials in the following file `~/.aws/credentials`.

```
[default]
aws_access_key_id = your_aws_access_key
aws_secret_access_key = your_aws_secret_access_key
```

1) Navigate into `aws` folder and run `terraform init`
2) Run `terraform plan`, this will output what will be executed
3) Run `terraform apply`, this will execute what your plan was (in this case add ec2 instance)


### Azure - Adding a DNS record
I set this up using the azure cli. Before you run this, follow the docuemntation on how to do so here https://www.terraform.io/docs/providers/azurerm/guides/azure_cli.html
1) Navigate into `azure` folder and run `terraform init`
2) Run `terraform plan`, this will output what will be executed
3) DO NOT RUN YET we dont want to make any changes to our DNS record accidentally. 
