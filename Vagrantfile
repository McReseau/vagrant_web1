# -*- mode: ruby -*-
# vi: set ft=ruby :
RAM = 1024
CPU = 1
HOSTNAME = "webserver"

Vagrant.configure("2") do |config|
  config.vm.box = "geerlingguy/centos7"
    config.vm.provider "virtualbox" do |v|
        v.name = HOSTNAME
        v.memory = RAM
        v.cpus = CPU
    end 
  config.vm.network "forwarded_port", guest: 80, host: 8080
  end
  