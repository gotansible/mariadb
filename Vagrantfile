# -*- mode: ruby -*-
# vi: set ft=ruby :
VAGRANT_VERSION = 2
Vagrant.configure(VAGRANT_VERSION) do |config|
	config.vm.define "mariadb" do |server|
		server.vm.box = "chef/centos-6.6"
		server.vm.hostname = "mariadb"
		server.vm.provision :ansible do |ansible|
			ansible.playbook = "test.yml"
		end
	end
end
