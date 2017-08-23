# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  #config.vm.box = "puppetlabs/centos-7.2-64-puppet"
  config.vm.box = "centos/7"
  config.vm.network "forwarded_port", guest: 80, host: 8087
  #config.vm.provision "shell", inline: "yum install -y epel-release && yum install -y ansible"
  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "ansible/site.yml"
    ansible.sudo = true
  end
  config.vbguest.auto_update = false
end
