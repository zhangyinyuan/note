
### centos 中 docker 开机启动

```
systemctl enable docker
```

### docker 镜像随着docker容器启动,如我的nginx dokcer中的容器id = 3a0dcde72fed
```
docker update --restart=always 3a0dcde72fed  
```
