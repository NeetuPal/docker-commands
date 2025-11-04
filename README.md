# docker-commands
## Deletes all "dangling" (untagged) images that are no longer needed.
```sh
docker rmi $(docker images -f "dangling=true" -q)
```
## Forcefully removes all containers, regardless of their state.
```sh
 docker rm -f $(docker ps -aq)
```
