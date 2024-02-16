Vagrant.configure("2") do |config|
  
  # Configuration de la VM ansible
  config.vm.define "ansible" do |ansible|
    ansible.vm.box = "generic/ubuntu2004"
    ansible.vm.hostname = "ansible"
    ansible.vm.network "private_network", ip: "10.10.20.3"
    ansible.vm.provider "libvirt" do |libvirt|
      libvirt.memory = 2048
      libvirt.cpus = 2
    end
  end

  # Configuration de la VM client1
  config.vm.define "client1" do |client1|
    client1.vm.box = "generic/ubuntu2004"
    client1.vm.hostname = "client1"
    client1.vm.network "private_network", ip: "10.10.20.4"
    client1.vm.provider "libvirt" do |libvirt|
      libvirt.memory = 1024
      libvirt.cpus = 1
    end
  end

  # Configuration de la VM client2
  config.vm.define "client2" do |client2|
    client2.vm.box = "generic/ubuntu2004"
    client2.vm.hostname = "client2"
    client2.vm.network "private_network", ip: "10.10.20.5"
    client2.vm.provider "libvirt" do |libvirt|
      libvirt.memory = 1024
      libvirt.cpus = 1
    end
  end

end
