# linux

## discovery

```
id
```

```
uname -a
```

## privesc

- the `adm` group can read log files

### view previously executed cron jobs

```bash
grep CRON /var/log/syslog
```
