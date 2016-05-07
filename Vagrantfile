Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty32"
  config.vm.box_url = "https://atlas.hashicorp.com/ubuntu/boxes/trusty32"
  
  config.vm.network :private_network, ip: "192.168.10.13"

  # set up apache, php, mysql
  config.vm.provision "ansible" do |ansible|
    ansible.playbook       = "playbook.yml"
    ansible.inventory_path = "inventory"
  end
end
