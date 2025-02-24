# Ubuntu 20.04 Machine with Terraform Engine

Easily creates a Vagrant Virtual Machine with Terraform platform.
Including some Terraform scrips ready-to-use.

<!-- Configuration in this directory creates set of VPC resources which may be sufficient for staging or production environment (look into [simple](../simple) for more simplified setup).

There are public, private, database, ElastiCache, intra (private w/o Internet access) subnets, and NAT Gateways created in each availability zone. -->

## Getting Started

### Prerequisites

To run this Virtual Machine you need first to install Vagrant by HashiCorp

* HashiCorp Vagrant Installation URL: [https://developer.hashicorp.com/vagrant/install](https://developer.hashicorp.com/vagrant/install)
 

* macOS Package manager
  ```bash
  brew tap hashicorp/tap
  brew install hashicorp/tap/hashicorp-vagrant
  ```


### Run the Virtal Machine

Inside the Vagrantfile directory, execute these commands:

```bash
$ vagrant init
$ vagrant up
```

When the VM is up, log in to the VM with:

```bash
$ vagrant ssh
```

<!-- Note that this example may create resources which can cost money (AWS Elastic IP, for example). Run `terraform destroy` when you don't need these resources. -->

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_vagrant"></a> [vagrant](#requirement\_vagrant) | >= 2.4.3 |
<!-- | <a name="requirement_awscli"></a> [awscli](#requirement\_awscli) | >= 1.18 |
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= v1.10.5 | -->

<!-- ## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 5.46 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_vpc"></a> [vpc](#module\_vpc) | ../../ | n/a |
| <a name="module_vpc_endpoints"></a> [vpc\_endpoints](#module\_vpc\_endpoints) | ../../modules/vpc-endpoints | n/a |
| <a name="module_vpc_endpoints_nocreate"></a> [vpc\_endpoints\_nocreate](#module\_vpc\_endpoints\_nocreate) | ../../modules/vpc-endpoints | n/a | -->
<!-- 
## Resources

| Name | Type |
|------|------|
| [aws_security_group.rds](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_availability_zones.available](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/availability_zones) | data source |
| [aws_iam_policy_document.dynamodb_endpoint_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.generic_endpoint_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |

## Inputs

No inputs.

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_cgw_arns"></a> [cgw\_arns](#output\_cgw\_arns) | List of ARNs of Customer Gateway |
| <a name="output_cgw_ids"></a> [cgw\_ids](#output\_cgw\_ids) | List of IDs of Customer Gateway |
| <a name="output_database_internet_gateway_route_id"></a> [database\_internet\_gateway\_route\_id](#output\_database\_internet\_gateway\_route\_id) | ID of the database internet gateway route |
| <a name="output_database_ipv6_egress_route_id"></a> [database\_ipv6\_egress\_route\_id](#output\_database\_ipv6\_egress\_route\_id) | ID of the database IPv6 egress route |
| <a name="output_database_nat_gateway_route_ids"></a> [database\_nat\_gateway\_route\_ids](#output\_database\_nat\_gateway\_route\_ids) | List of IDs of the database nat gateway route |
| <a name="output_database_network_acl_arn"></a> [database\_network\_acl\_arn](#output\_database\_network\_acl\_arn) | ARN of the database network ACL |
| <a name="output_database_network_acl_id"></a> [database\_network\_acl\_id](#output\_database\_network\_acl\_id) | ID of the database network ACL | -->
