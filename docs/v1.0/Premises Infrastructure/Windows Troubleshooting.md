# Windows- Troubleshooting Docker

## Run PowerShell in Admin Mode

In Start-Menu search for 'powershell'. To run PowerShell as administrator, right-click (or tap and hold, if you use a touchscreen) on the Windows PowerShell search result, and then click or tap "Run as administrator." (as shown in screenshot below)

## Windows 10



![Windows 10: Run PowerShell as Admin](/assets/images/e1bdd0c-Powershell.png)



## Windows 7



![Windows 7: Run PowerShell as Admin](/assets/images/c3dcf8b-PowerShell-Windows7.png)



## Restart Docker in PowerShell

Type following six commands in same order as given below:



## Error Code: open //./pipe/docker_engine: System cannot find file

error during connect: Get http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.29/version: open //./pipe/docker_engine: The system cannot find the file specified. In the default daemon configuration on Windows, the docker client must be run elevated to connect . This error may also indicate that the docker daemon is not running.



## Stuck in: "Waiting for an IP..." "Creating SSH Keys..."

Docker on Windows has a slew of problems. Here are few things you can try:


For more details refer to this article: https://github.com/docker/toolbox/issues/457
#####
```shell
net stop docker
net stop com.docker.service
taskkill /IM "dockerd.exe" /F
taskkill /IM "Docker for Windows.exe" /F
net start docker
net start com.docker.service
```

#####
```shell
docker-machine create default --virtualbox-no-vtx-check
docker-machine restart default



```

#####
```shell
First Disable AntiVirus
Next Disable FireWall
Next Run these commands
docker-machine rm default
docker-machine create --driver virtualbox --virtualbox-no-vtx-check default
```
