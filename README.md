# MAC终端重置mysql 密码

### 1.

##### 点击 系统偏好设置->MySQL -> Stop MySQL Server 关闭MySQL服务

### 2.

##### 打开终端输入 : cd /usr/local/mysql回车

##### sudo su 登入管理员权限定 回车

##### 输入以下命令来禁止mysql验证功能 ./mysqld_safe --skip-grant-tables & 回车

##### 此时MySQL会自动重启

### 3.

##### 重启后，输入./mysql

##### 回车后，输入命令 FLUSH PRIVILEGES;

### 4.

##### 回车后，输入命令 SET PASSWORD FOR 'root'@'localhost' = PASSWORD('你的新密码'); 或者 SET PASSWORD FOR 'root'@'localhost' = ('你的新密码')















