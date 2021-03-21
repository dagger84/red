# checks

_Ways to make sure your red teaming is more seamless._ 

## debugging payloads with `tcpdump`

### listen for incoming pings

```
tcpdump -i <interface> icmp
```

- Set up your payload to ping back, to check whether it works.
