Vagrant.configure("2") do |config|

  config.vm.provider "virtualbox" do |vb|
      vb.memory = "512"
  end
  config.vm.define "worker1" do |worker|
    worker.vm.box = "gusztavvargadr/docker-linux"
    worker.vm.network :private_network, ip: '172.20.20.11'
  end

  config.vm.define "worker2" do |worker|
    worker.vm.box = "gusztavvargadr/docker-linux"
    worker.vm.network :private_network, ip: '172.20.20.12'
  end

  config.vm.define "manager" do |manager|
    manager.vm.box = "gusztavvargadr/docker-linux"
    manager.vm.network :private_network, ip: '172.20.20.10'
  end
end
