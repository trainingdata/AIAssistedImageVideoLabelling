# Ubuntu- Troubleshooting Docker

## [Error: EACCES: permission denied, open 'db/trainingdata.db']

Or

## Mounted host volume is not writable from container

Your account's uid on host `id -u` is not the same as the uid of the user who is running the docker container. Try this:  

Now run docker image again. If you still get the same error try this:

Now run docker image again.
#####
```shell
sudo groupadd docker
sudo usermod -aG docker $USER
```

#####
```shell
chmod a+rwx -R db/


```
