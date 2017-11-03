Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.network "forwarded_port", guest: 1948, host: 8000
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
