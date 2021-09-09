# receptor_lab

Build lab:
```
# docker-compose up -d
```

Connect to mgmt-node:
```
# docker exec -it <container_id> /bin/bash
```

Receptor Commands
```
# receptorctl status
# receptorctl ping iso-node
# receptorctl traceroute iso-node
# receptorctl work submit hello --node iso-node -n 
# receptorctl work list --node iso-node
```

Receptor Status:
```
# receptorctl status
Node ID: mgmt-node
Version: 1.0.0
System CPU Count: 2
System Memory MiB: 1986

Connection   Cost
hop-node     1

Known Node   Known Connections
hop-node     {'iso-node': 1, 'mgmt-node': 1}
iso-node     {'hop-node': 1}
mgmt-node    {'hop-node': 1}

Route        Via
hop-node     hop-node
iso-node     hop-node

Node         Service   Type       Last Seen           Tags            Work Types
hop-node     control   Stream     2021-09-09 01:00:46 -               -
mgmt-node    control   Stream     2021-09-09 01:01:31 -               hello
iso-node     control   Stream     2021-09-09 01:00:46 -               -
```

Destroy lab:
```
# docker-compose down
```
