# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/xenial64"
    config.vm.box_url = "http://172.23.238.253/vagrant/boxes/xenial64v1.box"
      config.vm.network "forwarded_port", guest: 8080, host: 8080
        config.vm.provision :puppet
	  config.vm.provision "shell", inline: 'npm set registry http://172.23.238.253:4873/ -g'
	  end

