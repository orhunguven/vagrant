Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/trusty64"
    config.vm.hostname = "vagrant-flask"
    config.vm.network "forwarded_port", guest: 80, host: 8080
    ####ANSIBLE PROVISION####
    config.vm.provision "ansible_local" do |ansible|
        ansible.playbook = "provision/site.yml"
        ansible.verbose = "-vvv"
    end
end