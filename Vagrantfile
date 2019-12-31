Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/xenial64"
    config.vm.provision :shell, path: "vagrant.sh"
    config.vm.network "private_network", ip: "192.168.11.11"

    config.vm.synced_folder ".", "/vagrant", type: "nfs"
    config.vm.post_up_message = "Hello! Access the project at /vagrant"

    config.vm.provider "virtualbox" do |v|
        v.cpus = 2
        v.name = "project-" + Time.now.strftime("%L")
        v.memory = 2048
    end
end