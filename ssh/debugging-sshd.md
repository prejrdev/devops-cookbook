### Step 1
turn off the daemon by
```
service sshd stop
``` 

### Step 2
run sshd in debug mode 
```
/usr/sbin/sshd -ddd
```

### Step 3
and do something to reproduce the error to see if it shows up in stdout.

### Step 4
after terminating that process, just remember to start it up as a daemon again.
```
service sshd start
```
