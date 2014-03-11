Vagrant.configure("2") do |config|
  config.vm.box = "precise64"
  config.vm.box_url = "http://files.vagrantup.com/precise64.box"

  config.vm.network :private_network, ip: "192.168.33.10"
  config.vm.provision "shell", path: "provision.sh", privileged: false
  config.vm.synced_folder ".", "/vagrant", mount_options: ['dmode=775', 'fmode=664']
end
