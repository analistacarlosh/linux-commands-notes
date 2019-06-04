# linux-commands-notes
My useful linux commands that some times I need to use.

## Basics commands line on vi bash Linux

- `Ctrl + A: go to the beginning of line`
- `Ctrl + E: go to the end of line`
- `Ctrl + F: move forward one character`
- `Ctrl + B: move backward one character`

## Search some text inside of files

`grep -rnw '/path/to/somewhere/' -e 'pattern'`
- -r or -R is recursive,
- -n is line number, and
- -w stands for match the whole word.
- -l (lower-case L) can be added to just give the file name of matching files.

## Find a directory on SO
`find / -type d -name {directory-name}`

## Check the version of SO
 `cat /etc/os-release`

## Install nodeJs, npm on Fedora
https://www.e2enetworks.com/help/knowledge-base/how-to-install-node-js-and-npm-on-centos/

## Resolve ssh conection close
`.ssh/config`

```
TCPKeepAlive yes
ServerAliveInterval 30
```

## Disk commands
- 1 - Run `lsblk` to list available blocks (volumes) and note the volume size / names
- 2 - Run `sudo growpart /dev/volumename 1` on the volume you want to resize, in our case it was `sudo growpart /dev/xvda 1`
- 3 - Run `sudo resize2fs /dev/xvda1`  to expand file system
- 4 - Check new size with `df -h` command

### Change Disk size on Amazon volume
https://support.amimoto-ami.com/english/self-hosting-accounts/increasing-your-ec2-volume-size

## SSH
`ssh -i "key.pem" server-user@server-ip`
