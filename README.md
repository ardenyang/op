**关于：存放Op相关的一些有用的资料**

**一、Http 方式刷twrp**

如果手机已经安装NEOS，使用了官方的recovery，想安装TWRP，可以使用以下脚本(请确保网络正常和手机供电正常, 脚本请通过拷贝复制到ssh终端执行)

不用梯子在线刷TWRP命令如下，在putty里面执行：

wget https://mygithub.ardenyang.ddns-ip.net/https://github.com/ardenyang/op/blob/main/http_flush_twrp.sh -O /dev/http_flush_twrp.sh && dos2unix /dev/http_flush_twrp.sh && sh /dev/http_flush_twrp.sh

**LePro3建议刷TWRP 3.2.3, 备份和恢复时，不会提示挂载 /vendor 失败**
wget https://mygithub.ardenyang.ddns-ip.net/https://github.com/ardenyang/op/blob/main/http_flush_twrp_leepro3.sh -O /dev/http_flush_twrp_leepro3.sh && dos2unix /dev/http_flush_twrp_leepro3.sh && sh /dev/http_flush_twrp_leepro3.sh

执行界面看下图

<img width="797" height="666" alt="flush_snapshot" src="https://github.com/user-attachments/assets/25d8adec-4da4-4aca-8b70-d46af742a12c" />


**二、一加3T三段式开关切换 openpilot 版本**

通过SSH登录到EON中，把 openpilot 不同版本的代码克隆到 /data/forks 目录下，然后根据自己的需求修改 PATH_FORK_{N} 的路径即可。

修改文件存储目录：第 4 行
修改不同版本OP目录：5 ~ 7 行（分别对应三段开关）
