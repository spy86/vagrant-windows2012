# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|



  config.vm.define "webserver01" do |web01|
    web01.vm.box = "fujiiface/2012r2"
    web01.vm.hostname = "windows-webserver01"
    web01.vm.communicator = "winrm"
    web01.winrm.username = "vagrant"
    web01.winrm.password = "vagrant"
    web01.vm.network "private_network", ip: "192.168.57.3"
    web01.vm.provider "virtualbox" do |vb|
      vb.memory = 2048
      vb.cpus = 2
    end
  end
end