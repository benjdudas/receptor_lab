# receptor_lab

Build lab:
```
# docker-compose up -d
```

Connect to node1:
```
# docker exec -it <container_id> /bin/bash
```

Receptor Commands
```
# receptorctl status
# receptorctl ping node2
# receptorctl traceroute node2
```

Destroy lab:
```
# docker-compose down
```
