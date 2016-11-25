FGCI-ansible on openstack
=========================

Sets up an FGCI cluster in openstack

Sh/Could this be replaced with a PB - Pouta Blueprint?

Usage
------

 - provision at least three virtual machines
 - enter their names and ip addresses into hosts file and ssh.config
 - set selinux to disabled and reboot

Differences
-----------

 - using DHCP/PXE is difficult
 - no need for any roles which only apply to hardware, like dell, smartd

Known Limitations:
------------------

 - The "reinstall" script doesn't work. How to tie this into openstack reprovision?
 - Inventory of the hosts should be dynamic - so that one doesn't have to enter IP addresses into the hosts files or ssh.config
