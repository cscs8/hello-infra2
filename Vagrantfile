Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.provision "docker" do |d|
    d.build_image "/vagrant", args: "-t cs8/my-bash"
    d.run "cs8/my-bash", args: "-d -t -v /vagrant:/tmp/shared"
  end
end
