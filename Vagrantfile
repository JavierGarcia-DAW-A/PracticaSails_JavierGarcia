Vagrant.configure("2") do |config|
config.vm.box = "debian/bullseye64"

config.vm.network "private_network", ip: "192.168.56.10"

config.vm.synced_folder ".", "/var/www/laravel", owner: "vagrant", group: "vagrant"

config.vm.provider "virtualbox" do |vb|
vb.memory = "2048"
vb.cpus = 2
end
end