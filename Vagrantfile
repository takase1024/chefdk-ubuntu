
$script = <<SCRIPT

# Chef Development Kit Install(For CentOS)
#sudo yum -y localinstall https://opscode-omnibus-packages.s3.amazonaws.com/el/6/x86_64/chefdk-0.2.0-2.el6.x86_64.rpm

# Chef Development Kit Install(For Ubuntu)
wget https://opscode-omnibus-packages.s3.amazonaws.com/ubuntu/12.04/x86_64/chefdk_0.2.0-2_amd64.deb
sudo dpkg -i ./chefdk_0.2.0-2_amd64.deb

SCRIPT

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

#  config.vm.box = "CentOS_6_5_lyricalsoftware"
#  config.vm.box_url = "http://www.lyricalsoftware.com/downloads/centos65.box"

  config.vm.box = "Ubuntu_14_04_amd64"
  config.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box"

  config.vm.provision :shell, inline: $script

end
