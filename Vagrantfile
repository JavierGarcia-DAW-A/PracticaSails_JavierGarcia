Vagrant.configure("2") do |config|

  config.vm.box = "debian/bullseye64"

  config.vm.network "private_network", ip: "192.168.56.10"

  config.vm.synced_folder ".", "/var/www/laravel",
    owner: "vagrant",
    group: "vagrant",
    mount_options: ["dmode=775", "fmode=664"]

  config.vm.provider "virtualbox" do |vb|
    vb.name = "laravel-bullseye"
    vb.memory = 6144
    vb.cpus = 3 
  end

  config.vm.boot_timeout = 600
end

