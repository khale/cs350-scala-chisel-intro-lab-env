Vagrant.configure("2") do |config|

  config.vm.box = "mrlesmithjr/bionic64-desktop"
  config.vm.synced_folder ".", "/home/vagrant/lab3"
  config.vm.provision :shell, path: "https://gist.githubusercontent.com/khale/32ee31cb6840035b83419fda9e2f5e52/raw/8c73bb1631baa345fc69580f48ec2316e9f6f1ed/cs350-lab3-vagrant-bootstrap.sh"

  config.vm.provider "vmware_desktop" do |v|
    v.gui = true
  end

  config.vm.provider "virtualbox" do |v|
    v.gui = true
  end

end
