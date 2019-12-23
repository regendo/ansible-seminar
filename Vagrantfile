# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.
  config.ssh.insert_key = false

  config.vm.define "vagrant1" do |vagrant|
    vagrant.vm.box = "ubuntu/bionic64"
    vagrant.vm.network "forwarded_port", guest: 80, host: 8180, host_ip: "127.0.0.1"
    vagrant.vm.network "forwarded_port", guest: 443, host: 8143, host_ip: "127.0.0.1"
  end

  config.vm.define "vagrant2" do |vagrant|
    vagrant.vm.box = "ubuntu/bionic64"
    vagrant.vm.network "forwarded_port", guest: 80, host: 8280, host_ip: "127.0.0.1"
    vagrant.vm.network "forwarded_port", guest: 443, host: 8243, host_ip: "127.0.0.1"
  end

  config.vm.define "vagrant3" do |vagrant|
    vagrant.vm.box = "ubuntu/bionic64"
    vagrant.vm.network "forwarded_port", guest: 80, host: 8380, host_ip: "127.0.0.1"
    vagrant.vm.network "forwarded_port", guest: 443, host: 8343, host_ip: "127.0.0.1"
  end
end
