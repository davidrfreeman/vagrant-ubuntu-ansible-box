Vagrant.configure("2") do |cfg|
  compatibility__mode = "2"
  cfg.vm.box = "ubuntu/bionic64"
  cfg.vm.network = "forwarded_port", guest 80: host: 9000
  cfg.vm.network = "forwarded_port", guest 8080: host: 8080

  cfg.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbooks/main.yml"
    ansible.verbose = "vvvv"
  end
end