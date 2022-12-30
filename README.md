# Workgroup_Hyper-V
Companion commands from the video "Remotely Manage Workgroup Hyper-V Server 2019 Tutorial"

Get-NetAdapter| Get-NetConnectionProfile

Set-NetConnectionProfile -InterfaceAlias "vEthernet (LAN)" -NetworkCategory Private

Enable-PSRemoting

Enable-WSManCredSSP -Role server

APPWIZ.CPL

Start-Service -Name winrm

Set-Item WSMan:\localhost\Client\TrustedHosts -Value ST-HYP01.local

Stop-Service -Name winrm

Invoke-Command {WHOAMI} -Computername ST-HYP01.Local -Credential ST-HYP01\Administrator

Start-Service -Name winrm

Get-Item WSMan: \localhost\Client\TrustedHosts

GPEDIT.MSC

https://youtu.be/LEZSgWL6SZY
![](https://github.com/ShotokuTech/Workgroup_Hyper-V/blob/main/hyper-v%20workgroup.png)
