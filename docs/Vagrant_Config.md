# Vagrant Configuration

To add various configurations to vagrant, specify it in the config.

```
vagrant.configure('2') do |config|
    config.vm.box = 'ubuntu/xenial64'
    config.vm.provision :shell, path: "vagrant.sh"
    config.vm.network "private_network", ip: "192.168.11.11"
    ...
    ...
    ...
```



#### List of Configurations

- **config.vm.base_mac** (string) - The MAC address to be assigned to the default NAT interface on the guest.
_Support for this option is provider dependent_
<br/>

- **config.vm.base_address** (string) - The IP address to be assigned to the default NAT interface on the guest.
_Support for this option is provider dependent_
<br />

- **config.vm.boot_timeout** (string) - The time in seconds that Vagrant will wait for the machine to boot and be accessible. By default this is 300 seconds.
<br />



https://www.vagrantup.com/docs/vagrantfile/machine_settings.html#config-vm-base_address