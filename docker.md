
### centos 中 docker 开机启动

```
systemctl enable docker
```

### docker 镜像随着docker容器启动,如我的nginx在dokcer中的容器id = 3a0dcde72fed
```
docker update --restart=always 3a0dcde72fed  
```

### 查看docker仓库中redis的版本
```
docker search redis
```
### docker 安装命令使用apt-get,apt-get 更新
```
apt-get update
```

### docker 安装 vim
```
apt-get install -y vim
```


