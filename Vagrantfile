Vagrant.configure("2") do |config|
    config.vm.provider "virtualbox" do |vb|
      vb.name = "projeto05"
      vb.memory = 2048
      vb.cpus = 2
    end
  
    config.vm.box = "hashicorp/bionic64"
    config.vm.network "public_network", ip: "10.30.20.58"
  
    config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    end
  end
