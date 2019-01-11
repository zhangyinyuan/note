
- ### centos 中 docker 开机启动

```
systemctl enable docker
```

- ### docker 镜像随着docker容器启动,如我的nginx在dokcer中的容器id = 3a0dcde72fed
```
docker update --restart=always 3a0dcde72fed  
```

- ### 查看docker仓库中redis的版本
```
docker search redis
```
- ### docker 安装命令使用apt-get,apt-get 更新
```
apt-get update
```

- ### docker 安装 vim
```
apt-get install -y vim
```

- ### docker 容器中配置java环境
```
vim ~/.bashrc
export JAVA_HOME=/usr/lib/jvm/jdk1.8.0_121  ## 这里要注意目录要换成自己解压的jdk 目录
export JRE_HOME=${JAVA_HOME}/jre  
export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib  
export PATH=${JAVA_HOME}/bin:$PATH 
```

- ### 使得环境变量马上生效
```
source ~/.bashrc
```
- ### 安装 ifconfig 
```
apt-get install -y net-tools 
```
- ### 安装 ping
```
apt-get install -y iputils-ping
```
- ### 指定的容器修改 host,如容器的名称为 nginx
```
docker exec nginx /bin/sh -c "echo 127.0.0.1 nginx >> /etc/hosts"
```
