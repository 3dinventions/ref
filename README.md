# ref
A super simple bash script to create command references.  I have a hard time remembering commands so I made an easy searchable glossary of commands.  When I come across a command that I often forget, I add it to my reference glossary.  This script allows you to quickly search for command keywords or descriptions.

Usage:

Add a future command reference:
>ref a "-sync folders archive,verbose,human: rsync -avh source destination"

Search repository of references for keyword:
ref "sync"
> -sync folders archive,verbose,human: rsync -avh source destination

List all references:
ref l
> -find hosts on network: nmap -sP 192.168.0.1/24
> -external ip address: curl icanhazip.com
> -add user to sudo file: su -; usermod -aG sudo USER
> -find location of executable: whereis
> -borgmatic backup: sudo borgmatic create --verbosity 1 --list --stats
> -mount partition: sudo mount /dev/sdx /mnt/mountpoint
> -sync folders archive,verbose,human: rsync -avh source destination
> -change samba password: sudo smbpasswd -a user
> -symlink: /destination/folder_or_file name_of_link
> -service staus log: sudo journalctl -fu servicename
> -view permissions: ls -l file or folder
> -search running processes: ps cax | grep "borg"

Installation:
Copy ref to ~/.local/bin
chmod +x ~/.local/bin/ref
