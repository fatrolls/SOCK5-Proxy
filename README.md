# SOCK5-Proxy
SOCKS5 Proxy all communications on your machine.

======================================================== <br>
# Description
======================================================== <br>
```
Encrypt selected network traffic using a SOCKS 5 connection.
The project contains a service compatible executable "RedirectToSocks5.exe", that will redirect all outgoing network traffic
to a SOCKS 5 tunnel.
Also contains "tunnel.exe" that can send commands to the service
```

======================================================== <br>
# Requirements
======================================================== <br>
```
Visual studio redistribuitables :
	https://aka.ms/vs/16/release/vc_redist.x64.exe
A working SOCKS 5 tunnel
	ssh.exe -i ec2keypai2.pem ec2-user@3.22.221.46 -D 5556
```

======================================================== <br>
# Instalation
======================================================== <br>
```
Select a destination directory you wish the service to run from. Copy files to destination directory
Use ServiceRegister.bat to register the service
```

======================================================== <br>
# Usage
======================================================== <br>
```
Make sure you edit "tunnel.cfg" that will be located near "RedirectToSocks5.exe". 
Configuration values will be loaded on startup and can not be changed unless you restart the service.
Use "ServiceStart.bat" to start the service

You can use tunnel.exe to send commands to the service. Ex : start redirecting traffic, stop, load new rules
```
