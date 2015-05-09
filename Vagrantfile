# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "puppetlabs/ubuntu-12.04-64-puppet"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = 1024
    vb.cpus = 2
  end

  config.vm.network "forwarded_port", guest: 8000, host: 8000

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "challenge.yml"
  end

end
