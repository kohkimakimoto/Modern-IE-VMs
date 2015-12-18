# -*- mode: ruby -*-
# vi: set ft=ruby :

#
# see
# http://www.vagrantbox.es/
#

Vagrant.configure(2) do |config|

%w{
    win7-ie8
    win7-ie9
    win7-ie10
    win7-ie11
  }.each_with_index do |platform, index|
      config.vm.define platform do |c|
          c.vm.box = "http://aka.ms/vagrant-#{platform}"
          c.vm.provider :virtualbox do |vb|
            vb.gui = true
          end
      end
  end
end
