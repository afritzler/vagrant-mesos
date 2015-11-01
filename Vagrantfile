Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.hostname = "node1"
  config.vm.provision "shell" do |host|
      host.inline = "apt-get update -y; apt-get install -y software-properties-common; apt-add-repository ppa:ansible/ansible; apt-get update -y; apt-get install -y ansible"
      host.privileged = true
  end
end
