安装可选服务
服务
programdata/ssh/comfig
ssh-keygen -t rsa
Host deskcp
    HostName 192.168.1.102
    Port 22
    User sijianxin
scp .\id_rsa.pub desktp:./.ssh/authorized_keys