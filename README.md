# docker-commands
small and simple docker commands


## Copy a file from docker container to your local machine

```bash
  docker container cp <name-of-container>:/<path-to-the-file> <location-to-copy-file> 
```
Example: 

```bash 
  docker container cp mycontainer:/opt/data.json .
```

- - -
