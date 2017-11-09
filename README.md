# rabbitmqnotes
rabbitmq notes


## CentOS 安装

`安装erlang`

```shell
yum install erlang
```

```shell
yum install rabbitmq-server
```

## 常用命令

```shell
# 启动服务
service rabbitmq-server start

# 加入开机启动
chkconfig rabbitmq-server on

# 查看节点状态
rabbitmqctl status

# 查看virtual host
rabbitmqctl list_vhosts

# 添加virtual host
rabbitmqctl add_vhost <vhost_name>

# 查看用户列表
rabbitmqctl list_users

# 查看所有队列
rabbitmqctl list_queues

# 添加权限
rabbitmqctl set_permissions [-p vhost] {user} {conf} {write} {read}
```