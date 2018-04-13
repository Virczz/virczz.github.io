<!DOCTYPE html>
<html>

<head>
<meta charset="utf-8">

# RabbitMQ 简单使用步骤
参考 [Net分布式系统之四：RabbitMQ消息队列应用](https://www.cnblogs.com/Andon_liu/p/5401961.html)

- 安装ErLang运行环境 [下载和安装 RabbitMQ](http://www.rabbitmq.com/download.html)
- 检查环境变量，cmd> erl
- 安装RabbitMQ
- 启用web管理插件 *rabbitmq-plugins enable rabbitmq_management*

启动RabbitMQ 
1. cmd进入到RabbitMQ安装目录下\sbin\
2. rabbitmq-server on
rabbit-server start
3. 开启防火墙入站规则的端口 5672&15672
4. 创建一个账号
    rabbitmqctl add_user test test
    rabbitmqctl set_user_tags test administrator<br>rabbitmqctl set_permissions -p / test ".*" ".*" ".*"
5. 本机地址访问 http://localhost:15672/


