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