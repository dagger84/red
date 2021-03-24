# smb

## terms

- **NetBIOS name**. the NetBIOS server `//<netbios name>` that _may or may not_ be the server's IP address

## metasploit

- `auxiliary/scanner/smb/smb_version`. SMB version detection

## smbclient

### modifiers

#### anonymous/null authentication
- If no password is supplied at the prompt, then anonymous login is used.

#### force IP address (e.g. if NetBIOS name unknown)
- `-I <a.b.c.d>`. supply the IP address of the server to connect to.

### commands

#### list services

```
smbclient -L <netbios name>
```

- `-L`. list what services are available on the SMB server.

## smbmap

### modifiers

- `-H <ip>`. IP of SMB server host.
- `-u <username>`. username; **if omitted, null session is assumed**.
- `-p (<password>|<ntlm hash>)`. password or NTLM hash.
- `[-s <share>]`. specify a share; default: `C$`
- `[-d <domain>]`. domain name; default: `WORKGROUP`
- `[-P <port>]`. port; default: `445`

### commands
- `-R <path>`. recursive search.
- `-A (<pattern>|<file name>)`. retrieve files that match `<pattern>`.

## shopping list
- `Groups.xml`. Group Policy Preferences configuration file that contains encrypted passwords with a publicly available key.
