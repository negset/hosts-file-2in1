# hosts-file-2in1
flashable zip script to backup &amp; restore hosts file.

## Usage
1. Download the latest zip from [here](https://github.com/negset/hosts-file-2in1/releases/latest).
1. Copy zip to your device storage.
1. Flash zip via recovery before flashing a new ROM to backup the hosts file.
1. Flash zip again after flashing a new ROM to restore the hosts file.

### Backup Mode
If there is no backup, the script automatically switches to the backup mode.  
Hosts file will be backed up in the same location as the zip.
```
/system/etc/hosts -> {path-to-zip}/hosts.bak
```

### Restore Mode
If there is a backup, the script automatically switches to the restore mode.  
Hosts file will be restored to the system partition and set to the correct permissions.
```
{path-to-zip}/hosts.bak -> /system/etc/hosts
```
