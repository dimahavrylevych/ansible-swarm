Vagrant.configure("2") do |config|
  config.ssh.insert_key = false

  config.vm.define "master1" do |master|
    master.vm.box = "centos/7"
  	master.vm.network "private_network", ip: "192.168.61.10"
  	master.vm.hostname = "master1.test"
  end

  config.vm.define "worker1" do |worker|
    worker.vm.box = "centos/7"
  	worker.vm.network "private_network", ip: "192.168.61.11"
  	worker.vm.hostname = "worker.test"
  end
end
