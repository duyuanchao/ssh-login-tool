# ssh 
This is a SSH login tool

![alt text](image/ssh-login-tool.png)



## Run

1. git clone 
```
git clone https://github.com/duyuanchao/ssh-login-tool.git
```

2. modified login info in `password.lst`, all the username and password is saved in plaintext. The format is:
```
index:IP:port:user:password:description
1:192.168.88.130:22:root:passwd:svr_1
2:192.168.88.130:3000:user:passwd:svr_1-3000
3:192.168.88.4:22:root:passwd:svr_2
```  
3. add alias to your bashrc(`~/.bashrc`) or zshrc(`~/.zshrc`)
```
alias s='bash /path/to/folder/ssh-login-tool/server_login.sh'
```



### 二.配置
- 密码文件配置:

序号:IP:端口:用户:密码:说明
1:192.168.88.128:22:root:toor:虚拟机web服务器

- 密钥文件放在keys文件夹下,密码位置写成密钥文件名,文件名必须以.pem结尾
