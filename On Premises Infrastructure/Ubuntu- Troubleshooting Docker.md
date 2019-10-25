---
title: "Ubuntu: Troubleshooting Docker"
excerpt: ""
---
[block:api-header]
{
  "title": "[Error: EACCES: permission denied, open 'db/trainingdata.db']"
}
[/block]
Or
[block:api-header]
{
  "title": "Mounted host volume is not writable from container"
}
[/block]
Your account's uid on host `id -u` is not the same as the uid of the user who is running the docker container. Try this:  
[block:code]
{
  "codes": [
    {
      "code": "sudo groupadd docker\nsudo usermod -aG docker $USER",
      "language": "shell"
    }
  ]
}
[/block]
Now run docker image again. If you still get the same error try this:
[block:code]
{
  "codes": [
    {
      "code": "chmod a+rwx -R db/\n\n",
      "language": "shell"
    }
  ]
}
[/block]
Now run docker image again.