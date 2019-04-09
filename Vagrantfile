Vagrant.configure("2") do |config|

    config.vm.define "macosx-test"
    config.vm.box = "yzgyyang/macOS-10.14"

    config.vm.provider :virtualbox do |virtualbox|
        virtualbox.name = "macosx-test"
        #virtualbox.gui = true
        virtualbox.memory = 1024
        virtualbox.cpus = 2

        # Forward DNS resolver from host (vagrant dns) to box
        virtualbox.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
    end

end