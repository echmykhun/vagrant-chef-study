Vagrant::Config.run do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.provision :chef_solo do |chef|
    chef.cookbooks_path = "cookbooks"
    chef.add_recipe "bootstrap"
    chef.log_level = :debug
  end
end