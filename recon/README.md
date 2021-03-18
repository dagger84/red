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

|port|protocol|service |
|:--:|:------:|:------:|
|53  |UDP     |DNS     |
|88  |UDP     |Kerberos|
|445 |TCP     |SMB     |
