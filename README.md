# mikrotik-dyndns
Mikrotik RB750 script for updating dynamic ip-address at dy.fi

## Prerequisites

1. Create an account at http://dy.fi
2. Add a new host

### A brief introduction to dy.fi

dy.fi is a free dynamic DNS service offered exclusively for Finnish users.
It provides you a short domain name like 'yourname.dy.fi', which can be
pointed to the dynamic IP address of your home system (for running an FTP or
web server at home, or SSH/VNC remote use), or forwarded to your home page
which has a long and hard-to-remember URL.

## Instructions

1. Create a script with a name 'dyndns'
2. Schedule it to run once per hour
```
/system scheduler add name=run-1h interval=1h on-event=dyndns
```

**NOTE: Do NOT use character '$' in the  password, it will break the script.** 
