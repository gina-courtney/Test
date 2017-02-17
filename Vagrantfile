# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
	config.vm.define "box1" do |box1|
		box1.vm.box="ubuntu/trusty64"
		box1.vm.network :forwarded_port, guest: 22, host: 7955
		box1.vm.network :private_network, ip: "192.168.56.101"
	
	end	

	config.vm.define "box2" do |box2|
		box2.vm.box="hashicorp/precise64"
		box2.vm.network :forwarded_port, guest: 22, host: 7440
		box2.vm.network :private_network, ip: "192.168.56.102"
	end
