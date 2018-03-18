List documentation here


TODO:

1. Fix so vagrant can deal with mounting volumes. Issues are related to differences in 
kernel-devel versions of the vagrant boxes that cause fail on guestaddition update.
2. This system is currently not set up to build kernel modules.
Please install the Linux kernel "header" files matching the current kernel
3. vagrant plugin install vagrant-registration
4. vagrant plugin install vagrant-vbguest
5. vagrant plugin install vagrant-hostmanager
6. Install jre and visualvm
7. Install JDK
8. Prepare scripts that run before ansible to update kernel on CentOS7
	a. sudo yum update -y
	b. sudo yum install grub2-tools
	c. sudo yum install -y kernel*
	d. sudo mv -f /boot/grub2/grub.cfg /boot/grub2/grub.cfg-old
	e. sudo grub2-mkconfig -o /boot/grub2/grub.cfg
	f. sudo grub2-set-default 0
	g. reboot
9. vagrant plugin install vagrant-reload
