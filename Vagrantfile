Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"

  # config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.synced_folder "brave-hello", "/workspace"
 
  config.vm.provision "docker" do |d|
    d.build_image "/vagrant/builder", args: "-t builder"
  end
end
