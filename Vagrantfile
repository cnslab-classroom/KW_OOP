# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip: "192.168.56.100"
  config.vm.hostname = "cs7777"
  config.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        vb.cpus = 2
  end
  config.vm.provision "shell", inline: "sudo apt-get install tmux vim git -y"
  config.vm.provision "shell", inline: "wget https://download.oracle.com/java/18/latest/jdk-18_linux-x64_bin.deb"
  config.vm.provision "shell", inline: "sudo apt install ./jdk-18_linux-x64_bin.deb -y"
  config.vm.provision "shell", inline: "wget https://raw.githubusercontent.com/cnslab-kangwoon/KW_OOP/main/.vimrc -O /home/vagrant/.vimrc"
  config.vm.provision "shell", inline: "echo 'export JAVA_HOME=/usr/lib/jvm/jdk-18' >> /home/vagrant/.bashrc"
  config.vm.provision "shell", inline: "echo 'export PATH=$PATH:$JAVA_HOME/bin' >> /home/vagrant/.bashrc"

end
