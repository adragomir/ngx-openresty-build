# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|

  config.vm.define :sl65_64 do |sl65_64|
    sl65_64.vm.box     = 'centos66-hansode'
    sl65_64.vm.box_url = 'https://vagrantcloud.com/hansode/boxes/centos-6.6-x86_64/versions/0.1.0/providers/virtualbox.box' 
    sl65_64.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "512", "--cpus", "4"]
      vb.customize ["modifyvm", :id, "--nictype1", "virtio"]
      vb.customize ["modifyvm", :id, "--hpet", "on"]
    end
  end
  config.vm.define :trusty_64 do |trusty_64|
    trusty_64.vm.box = "trusty_64"
    trusty_64.vm.box_url = "http://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box"
    trusty_64.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "512", "--cpus", "2"]
      vb.customize ["modifyvm", :id, "--nictype1", "virtio"]
      vb.customize ["modifyvm", :id, "--hpet", "on"]
    end
  end
end
