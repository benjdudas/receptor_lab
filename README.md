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
# receptorctl ping node2
# receptorctl traceroute node2
# receptorctl work submit hello --node iso-node -n 
# receptorctl work list --node iso-node
```

Destroy lab:
```
# docker-compose down
```
