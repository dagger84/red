# recon

## initial scans

### default
```
nmap -sC -sV -oA <output prefix>
```

- `-sC`. default scripts
- `-sV`. enumerate versions
- `-oA`. output all formats (`nmap`, `gnmap`, `xml`)

### scan ports with safe scripts
```
nmap --script safe [...] -p[ports]
```

## port map

|port|service |
|:--:|:------:|
|53  |DNS     |
|88  |Kerberos|
|445 |SMB     |
