---
title: "Windows: Troubleshooting Docker"
excerpt: ""
---
[block:api-header]
{
  "title": "Run PowerShell in Admin Mode"
}
[/block]
In Start-Menu search for 'powershell'. To run PowerShell as administrator, right-click (or tap and hold, if you use a touchscreen) on the Windows PowerShell search result, and then click or tap "Run as administrator." (as shown in screenshot below)
[block:api-header]
{
  "title": "Windows 10"
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e1bdd0c-Powershell.png",
        "Powershell.png",
        429,
        565,
        "#dedee4"
      ],
      "caption": "Windows 10: Run PowerShell as Admin"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Windows 7"
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/c3dcf8b-PowerShell-Windows7.png",
        "PowerShell-Windows7.png",
        427,
        508,
        "#d8e3e9"
      ],
      "caption": "Windows 7: Run PowerShell as Admin"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Restart Docker in PowerShell"
}
[/block]
Type following six commands in same order as given below:
[block:code]
{
  "codes": [
    {
      "code": "net stop docker\nnet stop com.docker.service\ntaskkill /IM \"dockerd.exe\" /F\ntaskkill /IM \"Docker for Windows.exe\" /F\nnet start docker\nnet start com.docker.service",
      "language": "shell"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Error Code: open //./pipe/docker_engine: System cannot find file"
}
[/block]
error during connect: Get http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.29/version: open //./pipe/docker_engine: The system cannot find the file specified. In the default daemon configuration on Windows, the docker client must be run elevated to connect . This error may also indicate that the docker daemon is not running.
[block:code]
{
  "codes": [
    {
      "code": "docker-machine create default --virtualbox-no-vtx-check\ndocker-machine restart default\n\n\n",
      "language": "shell"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Stuck in: \"Waiting for an IP...\" \"Creating SSH Keys...\""
}
[/block]
Docker on Windows has a slew of problems. Here are few things you can try:

[block:code]
{
  "codes": [
    {
      "code": "First Disable AntiVirus\nNext Disable FireWall\nNext Run these commands\ndocker-machine rm default\ndocker-machine create --driver virtualbox --virtualbox-no-vtx-check default",
      "language": "shell"
    }
  ]
}
[/block]
For more details refer to this article: https://github.com/docker/toolbox/issues/457