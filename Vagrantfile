# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "puppetlabs/ubuntu-12.04-64-puppet"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = 1024
    vb.cpus = 2
    vb.customize [ "guestproperty", "set", :id, "/VirtualBox/GuestAdd/VBoxService/--timesync-set-threshold", 10000 ]
    vb.customize [ "modifyvm", :id, "--natdnshostresolver1", "on"]
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "devbox.yml"
    # ansible.tags = "nodejs"
    # ansible.skip_tags = "ruby,node"
    # ansible.verbose =  'v'
  end

end
