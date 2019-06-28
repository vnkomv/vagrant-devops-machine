# VAGRANT DEVOPS MACHINE

A project to have a Ubuntu windows machine to be used for development with a Windows Machine. The machine primarly aim to be used as a [remote development environment with Visual Studio Code](https://code.visualstudio.com/docs/remote/remote-overview). This remote development environment is focus on automation with [Terraform](https://www.terraform.io/) and [Ansible](https://www.ansible.com/) and also plugins creation for them.
The machine has the following program installed:

- Terraform 0.12.2
- Packer 1.4.1
- Python 2.7.15
- Golang 1.12
- Ansible 2.8.0
- Python librairie pywinrm
- Python librairie pywinrm[kerberos]
- Python librairie pywinrm[credssp]

The machine has also the following configuration:

- Copy of the keypairs

## REQUIREMENTS

You need the following software installed on your machine

- [Vagrant](https://www.vagrantup.com/)
- [Vagrant plugin Nugrant ](https://github.com/maoueh/nugrant)
- [Vagrant plugin vagrant-vbguest](https://github.com/dotless-de/vagrant-vbguest)

## USAGE

- Clone the repository
- Copy the `.vagrantuser.exemple` file to `.vagrantuser`. Change the variables according to your needs.
- Make sure you meet the requirements, especially the vagrant plugins.
- Run `vagrant up`

## CONFIGURATION

The following variables allow the customization of the machine. All the variables are required unless stated otherwise.

- **local_sync_folder:** the folder where you will put your projects to be synchronised on the virtual machine.

- **ip_address:** the static ip adress that will be use for the machine.
