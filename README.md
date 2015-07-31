Vagrantfile for the automatic creation of an OpENer development environment
===========================================================================

Requirements
------------
* Oracle VirtualBox (available at https://www.virtualbox.org)
* Vagrant (available at https://www.vagrantup.com)
* ChefDK (available at https://downloads.chef.io/chef-dk)

How-To
------
* Install Oracle VirtualBox
* Install Vagrant
* Install ChefDK
* Run command 'vagrant install plugin vagrant-omnibus'
* Run command 'vagrant install plugin vagrant-berkshelf'
* Clone the repository into a new folder
* Run command 'vagrant up'

If you are doing this the first time, vagrant will download a Debian Jessie 64-bit basebox from Hashicorps Atlas service.
I created this machine myself, with the Packer configuration found at https://github.com/CapXilinx/packer-DebianJessie.
If you want to use your own basebox modify the Vagrantfile accordingly.

After the basebox is downloaded and provisioned you are ready to start.
Run the command 'vagrant ssh' to log in to a secure shell of the development machine.

The default user is 'vagrant', the password is also 'vagrant'.
The root password is 'vagrant'.

The OpENer repository should be already downloaded to /home/vagrant/OpENer.
