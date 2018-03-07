Vagrant.configure(2) do |config|
  config.vm.box = "bento/debian-9.3"
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "provision.yml"
  end
end
