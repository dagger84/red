# Memory corruption

## GDB (GNU Debugger)

- Attach to existing process; this avoids GDB changing settings such as disabling ASLR

```
gdb --pid=<pid>
```
