# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "joelhandwell/ubuntu_xenial64_vbguest"
  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.provider "virtualbox" do |v|
    v.memory = 8192
    v.cpus = 8
  end
  config.vm.provision "shell", path: "./setup.sh"
end
