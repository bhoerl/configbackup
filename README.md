# configbackup
A tool for automated device config backup<br>
(Python Version 2.x required)

## Install required python packages
`pip install pexpect requests tftpy scp`

## Basic usage
run `python check_coin_price.py --help`
```
Usage:
 configbackup.py --ftp -s <host> -u [username] -p [password] -f <file> -d <backup_dir> -c [custom_folder]
 configbackup.py --tftp -s <host> -d <backup_dir> -c [custom_folder]
 configbackup.py --http -s <host> -u [username] -p [password] -f <file> -d <backup_dir> -c [custom_folder]
 configbackup.py --https -s <host> -u [username] -p [password] -f <file> -d <backup_dir> -c [custom_folder]
 configbackup.py --scp -s <host> -u [username] -p [password] -f <file> -d <backup_dir> -c [custom_folder]
 configbackup.py --ssh-ios -s <host> -u <username> -p <password> -e [enable-password] -d <backup_dir> -c [custom_folder]
 configbackup.py --ssh-asa -s <host> -u <username> -p <password> -e [enable-password] -d <backup_dir> -c [custom_folder]
 configbackup.py --ssh-pix -s <host> -u <username> -p <password> -e [enable-password] -d <backup_dir> -c [custom_folder]
 configbackup.py --ssh-nxos -s <host> -u <username> -p <password> -e [enable-password] -d <backup_dir> -c [custom_folder]
 configbackup.py --ssh-iosxr -s <host> -u <username> -p <password> -e [enable-password] -d <backup_dir> -c [custom_folder]
 configbackup.py --telnet-ios -s <host> -u [username] -p <password> -e [enable-password] -d <backup_dir> -c [custom_folder]
 configbackup.py --telnet-pix -s <host> -u [username] -p <password> -e [enable-password] -d <backup_dir> -c [custom_folder]
 configbackup.py --ironport -s <host> -u <username> -p <password> -d <backup_dir> -c [custom_folder]

Options:
  -h, --help        show this help message and exit
  --ftp             ftp connect
  --tftp            tftp connect
  --http            http connect
  --https           https connect
  --scp             scp connect
  --ssh-ios         ssh connect for cisco ios (show startup-config)
  --ssh-asa         ssh connect for cisco asa (more system:running-config)
  --ssh-pix         ssh connect for cisco pix (show startup-config)
  --ssh-nxos        ssh connect for cisco nxos (show startup-config)
  --ssh-iosxr       ssh connect for cisco ios-xr (show running-config)
  --telnet-ios      telnet connect for cisco ios (show startup-config)
  --telnet-pix      telnet connect for cisco pix (show startup-config)
  --ironport        ssh connect and scp for cisco ironport (wsa/esa)
  -d BACKUPDIR      specify main backup directory
  -s HOSTNAME       hostname or ip address
  -u USER           username
  -p PASSWORD       password
  -e ENABLE         enable password
  -f FILENAME       filename or path
  -c CUSTOM_FOLDER  custom backup folder name, default is HOSTNAME
```
