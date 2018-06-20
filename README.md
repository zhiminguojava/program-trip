
数据库10038
1、grant all privileges on *.*  to  'root'@'%'  identified by 'youpassword'  with grant option;
flush privileges;
2、修改 /etc/mysql/mysql.conf.d  （ 老版本的是这个目录：/etc/mysql/my.conf ）
找到bind-address = 127.0.0.1这一行，改为bind-address = 0.0.0.0即可
如果方案1、2都不可行检查一下远程端口
