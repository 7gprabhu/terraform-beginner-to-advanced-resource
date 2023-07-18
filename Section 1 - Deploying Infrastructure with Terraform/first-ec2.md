### Documentation Referred:

https://registry.terraform.io/

https://registry.terraform.io/providers/hashicorp/aws/latest/docs

### first_ec2.tf

```sh
provider "aws" {
  region     = "us-east-1"
  access_key = "AKIAYREVECK6II2SQ7KA"
  secret_key = "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"
}

resource "aws_instance" "myec2" {
    ami = "ami-00c39f71452c08778"
    instance_type = "t2.micro"
}
```

### Commands:

```sh
terraform init
terraform plan
terraform apply
```
