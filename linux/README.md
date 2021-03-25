# linux

## discovery
- `id`
- `uname -a`

## privesc

### log files
- the `adm` group can read log files
- `grep CRON /var/log/syslog`. view previously executed cron jobs

## devices
- `pcspkr`. access the PC speaker

## pam.d
- `/etc/pam.d/system-auth`. look at account lockout policy.

## fail2ban
- `/etc/fail2ban/fail2ban.conf`. look at account lockout policy.

## lfi
- `/proc/self/status`. view the owner (UID) of a process if the only access is via LFI.
