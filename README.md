# mikrotik-dyndns
Mikrotik RB750 script for updating dynamic ip-address at dy.fi

Instructions

1. Create a script with a name 'dyndns'
2. Schedule it to run once per hour
```
/system scheduler add name=run-1h interval=1h on-event=dyndns
```
