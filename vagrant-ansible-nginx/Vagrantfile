Vagrant.configure("2") do |config|
    config.vm.box = "hashicorp/bionic64"
    config.vm.provider "virtualbox" do |v|
    v.name = "Marlon"
    end   
    config.vm.network "public_network"
    config.vm.provision  "ansible" do |ansible|
      ansible.compatibility_mode = "auto"
      ansible.playbook = "playbook.yml"
    end
end