# -*- mode: ruby -*-
# vi: set ft=ruby :

# Every Vagrant development environment requires a box. You can search for
# boxes at https://atlas.hashicorp.com/search.

BOX_IMAGE = "starboard/ubuntu-arm64-20.04.5"
BOX_VERSION = "20221120.20.40.0"

#BOX_IMAGE= "rethinc-oss/ubuntu-2204-arm64"
#BOX_VERSION = "20220819"

NODE_COUNT = 2

Vagrant.configure("2") do |config|
  
  (1..NODE_COUNT).each do |i|
    config.vm.define "node#{i}" do |subconfig|
      subconfig.vm.box = BOX_IMAGE
      subconfig.vm.box_version= BOX_VERSION
      subconfig.vm.hostname = "node#{i}"
    end
  end

end
