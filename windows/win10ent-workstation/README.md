# Windows Workstation

## Build vagrant image 

Update below parameters

```
"iso_checksum": "34887592ECC25B725A527748D31971F22C78C82B",
"iso_mirror": "D:\\home\\downloads\\windows10",
"iso_name": "windows10.iso",
```

packer build  -only=virtualbox-iso .\windows-10-win.json
