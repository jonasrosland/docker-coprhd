vagrant-coprhd
---------------

# Description

Vagrantfile to create a single node [CoprHD](coprhd.github.io) controller. CoprHD will be build from sources.

# Requirements
* 4 vCPU 
* 8 GB of free RAM
* Vagrant
* Virtualbox

# Usage
Either use the "Download ZIP" link on the right side of this page and unpack the zipfile somewhere on your computer, or clone using git: `git clone https://github.com/vchrisb/vagrant-coprhd.git`

Now open a shell and change directory to vagrant-coprhd

Finally issue `vagrant up` (if you have more than one Vagrant Provider on your machine run `vagrant up --provider virtualbox` instead)

Depending on your download bandwidth does the installation and build take some time.

Once Vagrant is done you should be able to connect to CoprHD a few minutes later by opening `https://192.168.100.10`. 

Username: `root`
Password: `ChangeMe`

Documentation for CoprHD is currently the same as the commercial ViPR Product:
https://community.emc.com/docs/DOC-41200

# Troubleshoot

If you experience an error please look at the logs. The CoprHD build process will download artifacts from the CoprHD Jenkins server and many other ones.
I've tested with `Vagrant 1.7.2` and `Virtualbox 4.3.28` on `Windows 7`.
