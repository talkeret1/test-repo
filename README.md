<a id="readme-top"></a>
# Vagrant VM: Ubuntu 20.04 with Terraform Engine
<br>

Easily creates a Vagrant Virtual Machine with Terraform platform.<br>
Including some ready-to-use <a href="#terraform-scripts">Terraform scripts</a>.
<br>
<br>
## Prerequisites

### Install Vagrant:

To run this Virtual Machine you need first to install Vagrant by HashiCorp

* HashiCorp Vagrant Installation URL: [https://developer.hashicorp.com/vagrant/install](https://developer.hashicorp.com/vagrant/install)
 
* Install from macOS Package manager:
  ```bash
  brew tap hashicorp/tap
  brew install hashicorp/tap/hashicorp-vagrant
  ```

### Define the connection to your AWS account:

Inside your [AWS Console](https://us-east-1.console.aws.amazon.com/):
1. Create an `AWS IAM User` with Permissions Policies: "`AdministratorAccess`" 
2. Create `CLI Access Key` and download the `.csv` file
3. Move the `.csv` file to the Vagrant directory
4. Remove Any other `.csv` files (exampleUser_accessKeys.csv)
<br>
<br>

## Getting Started

### Start the Virtal Machine:

Inside the Vagrant directory, execute these commands:

```bash
vagrant init
vagrant up
```

### Log into the Virtual Machine:

After the VM is up, log in to it:

```bash
vagrant ssh
```
<br>
Setup is done, Your Terraform Machine is ready!

Use `terraform version` to ensure that a the installation was successfull.<br>
<br>
<br>

## Ready-to-Use Terraform Scripts

Inside the VM there is a directory that shared with the host: `/vagrant/terrafrom/`<br>
Inside this folder you can find ready-to-use Terraform scripts.<br>
<br>

### Run the script:
Select your desired script from `/vagrant/terrafrom/` and run it:
```bash
cd 1*
terraform init
terraform apply
```

:heavy_exclamation_mark: Note that this action may create AWS resources which can cost money.<br>
<br>

### Destroy the script:
Remove all script resources:
```bash
terraform destroy
```
<br>

<a id="terraform-scripts"></a>
### Terraform Scripts List:

* [1-UbuntuInstance](/terraform/1-UbuntuInstance/README.md) - AWS Instance with Ubuntu 20.04
* [2-UbuntuWebServer](/terraform/2-UbuntuWebServer/README.md) - Ubuntu 20.04 with Apache2 HTTP Web Server

<p align="right">(<a href="#readme-top">back to top</a>)</p>
