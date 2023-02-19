# -*- mode: ruby -*-
# vi: set ft=ruby :
IMAGE_BOX="geerlingguy/centos7"
RAM = 1024
CPU = 1
HOSTNAME = "webserver"
PRIVATE_IP = "10.0.0.10"

Vagrant.configure("2") do |config|
  config.vm.box = IMAGE_BOX
    config.vm.provider "virtualbox" do |v|
        v.name = HOSTNAME
        v.memory = RAM
        v.cpus = CPU
    end 
  config.vm.network "private_network", ip: PRIVATE_IP
config.vm.network "forwarded_port", guest: 80, host: 8080
  end
  