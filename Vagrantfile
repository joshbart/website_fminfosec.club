Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.network :forwarded_port, guest: 80, host: 49179
  config.vm.network :forwarded_port, guest: 443, host: 49180
  config.vm.provision :shell, path: "apache/install.sh"
end
