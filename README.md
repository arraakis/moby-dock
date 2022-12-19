# docker-commands
small and simple docker commands


## Copy a file from docker container to your local machine

```bash
  docker container cp <name-of-container>:/<path-to-the-file> <location-to-copy-file> 
```
Example: 

```bash 
  docker container cp moby:/opt/data.json .
```

- - -


## How to mount host directory in Docker

```bash
  docker run -it --rm -v $(pwd):/opt/ moby bash
```
- - -


## How to analyze container logs

```bash
  docker logs 44153e72e7a3
```

--tail flag:
  - see the last 50 lines of the log
```bash
  docker logs --tail 50 44153e72e7a3
```

since flag:
  - see the last 50 lines of the log
```bash
  docker logs --since 10 44153e72e7a3
```


inspect: 
-  get a json format 

```bash
  docker inspect --format={{.LogPath}} 44153e72e7a3
```
returns the location of the log file. 

- - -
