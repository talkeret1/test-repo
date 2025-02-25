# Vagrant VM: Ubuntu 20.04 + Terraform Engine

Easily creates a Vagrant Virtual Machine with Terraform platform.
Includes some Terraform scrips ready-to-use.

<!-- Configuration in this directory creates set of VPC resources which may be sufficient for staging or production environment (look into [simple](../simple) for more simplified setup).

There are public, private, database, ElastiCache, intra (private w/o Internet access) subnets, and NAT Gateways created in each availability zone. -->

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

* Inside your [AWS Console](https://us-east-1.console.aws.amazon.com/):
1. Create an `AWS IAM User` with Permissions Policies: "`AdministratorAccess`" 
2. Create `CLI Access Key` and download the `.csv` file
3. Move the `.csv` file to the Vagrant directory
4. Remove Any other `.csv` files (exampleUser_accessKeys.csv)


## Getting Started

### Start the Virtal Machine

Inside the Vagrant directory, execute these commands:

```bash
$ vagrant init
$ vagrant up
```

### Log into the VM

When the VM is up, log in to the VM with:

```bash
$ vagrant ssh
```
Setup is done, Your Terraform Machine is ready!

Use `terraform version` to ensure that a the installation was successfull.

## Ready-to-Use Terraform Scripts

Inside the VM there is a shared folder with the host: `/vagrant/terrafrom/`

In this folder you can find ready-to-use Terraform scripts.

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [1-UbuntuInstance](/terraform/1-UbuntuInstance/README.md) - AWS Instance with Ubuntu 20.04
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)
