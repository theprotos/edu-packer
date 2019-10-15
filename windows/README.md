[Create/upload vagrant box](https://www.vagrantup.com/docs/vagrant-cloud/boxes/create.html)

[Windows automated setup](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/automate-windows-setup)


# win10workstation.json

## Build vagrant image 

Update below parameters in [win10workstation.json](win10workstation.json)

```
"autounattend": "answer_files/win10ent/Autounattend.xml",
"iso_checksum": "34887592ECC25B725A527748D31971F22C78C82B",
"iso_mirror": "D:\\home\\downloads\\windows10",
"iso_name": "windows10.iso",
```

```
packer build  -only=virtualbox-iso .\win10workstation.json
```