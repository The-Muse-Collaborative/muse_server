Vagrant.configure(2) do |config|
  config.vm.box = "bento/debian-9.3"
  config.vm.hostname = "muse-dev"
  config.vm.network :private_network, ip: "192.168.33.10"
  config.vm.provider "virtualbox" do |virtualbox|
    virtualbox.name = config.vm.hostname
  end
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "provision.yml"
  end
end
