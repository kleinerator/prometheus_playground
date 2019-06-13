# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"
  config.vm.network "forwarded_port", guest: 22, host: 2424, id: "ssh"
  config.vm.network "forwarded_port", guest: 9090, host: 9090
  config.vm.network "forwarded_port", guest: 9093, host: 9093
  config.vm.network "forwarded_port", guest: 3000, host: 3000

  config.vm.provider "virtualbox" do |vb|
    # Customize the amount of memory on the VM:
    vb.memory = "3092"
    vb.name = "prometheus"
  end

  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   #apt-get upgrade -y
  #   apt-get install -y aptitude python-minimal
  # SHELL

  # config.vm.provision "ansible" do |ansible|
  #   ansible.playbook = "prometheus.yml"
  # end

end
