# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-16.04"

  config.vm.network "private_network", ip: "10.10.10.10"
  config.vm.hostname = "ubuntu.local"

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.memory = "1024"
  end

  config.vm.provision :shell, :inline =>
    "/vagrant/ansible/provision.sh"
end