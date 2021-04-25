## gitlab系列

官网地址：http://about.gitlab.com

安装说明：http://about.gitlab.com/installation

## gitlab操作

- #### 初始化配置gitlab

  gitlab-ctl reconfigure

- #### 启动gitlab

  gitlab-ctl start

- 停止gitlob服务

  gitlab-ct stopl 

## 浏览器访问

访问Linux服务器IP地址即可，如果想访问EXTERNAL_URL指定的域名还需要配置域名服务器或本地hosts文件。

初次登陆时需要为gitlab的root用户设置密码。

1. 需要停止防火墙服务          （运维人员思考防火策略）
2. service  firewalld stop

账号密码