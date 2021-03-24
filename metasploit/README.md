# metasploit

## terminology

- **handler.** the process on the attacker or C2 machine that ensures a payload executes correctly
  - starts up a server to deliver the next stages of a staged payload
  - starts up a listener for final incoming connections
- **listener**. waits for an incoming connection from an exploited system.
- **payload**. the code that is run on the victim's computer.
- **loader/stager.** the small stub of code in shellcode that downloads a full payload.

## main commands
- `sessions`
- `search`

### using an exploit
- `show options`.
- `info`.
- `check`.
- `run`.

## meterpreter
- `getuid`. get the current user's id
- `sysinfo`
- `hashdump`
- `ps`
- `load`
  - `kiwi`
    
## mimikatz
- `lsa_dump_secrets`

## reference

- [What is a handler?](https://docs.rapid7.com/metasploit/working-with-payloads/)
- [How do staged payloads in metasploit work?](https://buffered.io/posts/staged-vs-stageless-handlers/)
- [Stageless metasploit payloads](https://blog.rapid7.com/2015/03/25/stageless-meterpreter-payloads/)
