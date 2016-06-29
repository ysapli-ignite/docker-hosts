# docker-hosts
Simple script that listens to docker start/stop/die events to add/remove containers to/from /etc/hosts so that they can be automatically adressed by their hostnames.

Just clone it and run it as root. If you want to disable it, run the following command as root:
```
ps aux | grep dock_event | grep -v grep | awk '{print $2}' | xargs kill
```
