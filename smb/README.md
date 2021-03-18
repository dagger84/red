# smb

## terms

- **NetBIOS name**. the NetBIOS server `//<netbios name>` that _may or may not_ be the server's IP address

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



