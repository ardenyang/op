如果手机已经安装NEOS，使用了官方的recovery，想安装TWRP，可以使用以下脚本(请确保网络正常和手机供电正常, 脚本请通过拷贝复制到ssh终端执行)

不用梯子在线刷TWRP命令如下，在putty里面执行：

wget https://mygithub.ardenyang.ddns-ip.net/https://github.com/ardenyang/op/blob/main/http_flush_twrp.sh -O /dev/http_flush_twrp.sh && dos2unix /dev/http_flush_twrp.sh && sh /dev/http_flush_twrp.sh

执行界面看下图
<img width="797" height="666" alt="flush_snapshot" src="https://github.com/user-attachments/assets/25d8adec-4da4-4aca-8b70-d46af742a12c" />
