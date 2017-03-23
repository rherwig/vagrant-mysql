# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.network "private_network", ip: "10.10.10.20"
  config.vm.hostname = "magento.local"

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.memory = "2048"
  end

  config.vm.provision :shell, :inline =>
    "/vagrant/ansible/provision.sh"
end
