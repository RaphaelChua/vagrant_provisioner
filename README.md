# Vagrant





##### To be able to run vagrant, turn hypervisor off and restart your computer.
```cmd
bcdedit /set hypervisorlaunchtype off
```

##### To be able to run docker, turn hypervisor on and restart your computer.
```cmd
bcdedit /set hypervisorlaunchtype auto
```