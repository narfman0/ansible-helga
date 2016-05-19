# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|
  config.vm.box = "glenux/jessie64-lxc"
  config.vm.hostname = "helga"
  # config.vm.network "public_network"
  config.vm.define :helga
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "provisioning/playbook.yml"
  end
end
