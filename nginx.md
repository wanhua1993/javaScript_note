### 查看mongodb运行状态
> netstat -lanp | grep "27017"
> netstat -n | awk '/^tcp/ {++S[$NF]} END {for(a in S) print a, S[a]}'
### 编辑文件
> vim 或者 vi
### 退出保存
> :wq + enter
### 重启系统配置文件
> source /etc/profile
### 查看磁盘使用情况
> df -h
### 添加用户
> adduser wanhua
> gpasswd -a wanhua sudo
> sudi visudo
> wanhua ALL=(ALL:ALL) ALL
### 无密码登录
> 
### 查看进程号 （nginx）
> ps -ef|grep nginx
### 启动 nginx
> /usr/local/nginx/sbin/nginx -c /usr/local//nginx/conf/nginx.conf
### 停止 nginx
> kill -QUIT + 进程号  kill -9 + 进程号

