## Providers

| Name | Version |
|------|---------|
| aws | n/a |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:-----:|
| aws\_amis | The AMI image to use (Debian 8) | `map` | <pre>{<br>  "ap-southeast-1": "ami-4e370d1c",<br>  "ap-southeast-2": "ami-e7c5bddd",<br>  "eu-west-1": "ami-971a65e0",<br>  "us-east-1": "ami-896d85e2",<br>  "us-west-1": "ami-21cf2565",<br>  "us-west-2": "ami-ed8eb7dd"<br>}</pre> | no |
| instance\_type | Size of the instance | `string` | `"t1.micro"` | no |
| ip\_whitelist | Whitelisted IP for SSH access | `string` | `"0.0.0.0/0"` | no |
| key\_name | Key pair to use | `string` | `"example"` | no |
| region | Credentials are read in through terraform.tfvars (not in git) AWS Region | `string` | `"us-west-1"` | no |

## Outputs

| Name | Description |
|------|-------------|
| EC2\_DNS\_name | n/a |
| EC2\_IP\_address | The EC2 instance |
| db\_instance\_address | n/a |
| db\_instance\_id | The RDS instance |

# hashi-chip-drupal
