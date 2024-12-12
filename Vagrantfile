Vagrant.configure("2") do |config|
  config.vm.provider "virtualbox" do |vb|
    vb.name = "ubuntu-01"
    vb.memory = 1024
    vb.cpus = 1
  end
  config.vm.box = "bento/ubuntu-20.04"
  config.vm.network "public_network", bridge: "wlp4s0"
  config.vm.synced_folder "hello/", "/home/vagrant/hello"
end
