Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"

  config.vm.hostname = "gitlab.local"

  config.vm.box_version = "20210208.0.0"
  config.vm.box_url = "https://vagrantcloud.com/ubuntu/bionic64"

  config.vm.network "forwarded_port", guest: 81, host: 8801
  config.vm.network "forwarded_port", guest: 22, host: 8022
  
  config.vm.network "private_network", ip: "192.168.33.44"
  
  config.vm.provider "virtualbox" do |v|
  v.gui = true
  v.memory = 4096
  # v.memory = 3072
  
  end
 
  config.vm.provision "shell", inline: <<-SHELL
  # Installation et configuration des dépendances nécessaires pour GitLab-ce
  apt-get update
  apt-get install -y curl openssh-server ca-certificates
 
  # Ajout du référentiel de packages GitLab-ce 
  curl  https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/script.deb.sh | sudo bash
  
  # Installation du package GitLab-ce
  # EXTERNAL_URL="http://gitlab.local" apt-get install gitlab-ce
  apt-get install gitlab-ce
  gitlab-ctl reconfigure
  SHELL

  # Installation pelican et packages optionnels
  config.vm.provision "shell", inline: <<-SHELL
  apt-get update
  apt-get install -y pelican
  SHELL

  # Installation markdown
  config.vm.provision "shell", inline: <<-SHELL
  apt-get update
  apt-get install -y markdown
  SHELL
  end
 
 
  