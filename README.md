# Information

Clone of [github.com/microsoft/linux-vm-tools](https://github.com/microsoft/linux-vm-tools).

The original repository is archived, forking it here just in case the original is deleted.


## Instructions

See [this](https://askubuntu.com/a/1251827/739717) StackOverflow answer for more info.

## In the linux guest

:warning: **Disable** "Auto Login" if you enabled it.

in a terminal execute:
```bash
wget https://raw.githubusercontent.com/ruizpauker/linux-vm-tools/master/ubuntu/18.04/install.sh
sudo chmod +x install.sh
sudo ./install.sh
```

## In the Windows host

In a Powershell console, execute:

```powershell
Set-VM -VMName <your_vm_name> -EnhancedSessionTransportType HvSocket
```
