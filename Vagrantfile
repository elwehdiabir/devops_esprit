Vagrant.configure("2") do |config|
  # Use Ubuntu 22.04 as base image
  config.vm.box = "bento/ubuntu-22.04"
  config.vm.boot_timeout = 600
  # test NODE
  config.vm.define "test" do |test|
    test.vm.hostname = "test1"

    # Network
    test.vm.network "private_network", ip: "192.168.56.10"

    # Resources
    test.vm.provider "virtualbox" do |vb|
      vb.memory = 4192
      vb.cpus = 2
    end  
  end

end