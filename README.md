# NPS
NPS内网穿透项目（带Web控制端）

安装Linux服务端

Git下载服务端源码到公网IP服务器上
```
git https://github.com/SocksReckless/NPS/blob/main/linux_amd64_server.tar
```

进入源码目录
```
cd linux_amd64_server
```

安装NPS服务端
```
./nps install
```

安装完成后浏览器打开
http://IP:8080

默认账户名密码
admin
password

安装完成后修改/etc/nps/conf/nps.conf文件
```
vim /etc/nps/conf/nps.conf
```

修改key后面的数值，随意
auth_key=
auth_crypt_key =

修改完成后，重启NPS
```
nps restart
```

改动任何配置文件都要进行重启
