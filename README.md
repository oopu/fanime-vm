# fanime-vm
Dev VM for working with fanime-* repositories. Using this to develop in these repositories is strongly recommended.

## Setup Requirements
This project is based on Vagrant (v1.8.6) and VirtualBox (v5.1) 
* [Installing Vagrant](https://www.vagrantup.com/docs/installation/)
* [Installing VirtualBox](https://www.virtualbox.org/)

## Getting Started
* Install the dependencies above
* Clone this repository
* Navigate to the project repo
* Type `vagrant up`

A VM will be created which you can subsequently access through VirtualBox or directly by then hitting `vagrant ssh`.
The user is `vagrant`. The `vagrant ssh` command will tell you more about how you can SSH into the created VM with something
else, like PuTTY if you're on Windows.


## Where are my files?
This VM is configured to sync the `/home/vagrant/projects` directory within the VM with a folder it will create in this
project's directory, named `fanime-vm-projects`. The synchronization protocol is automatically chosen based on environment.

If you wish to change this, edit the Vagrantfile in this project and type `vagrant reload`.
