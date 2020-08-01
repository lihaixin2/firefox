## firefox介绍

基于ubuntu:16.04 配置x11和novnc 服务和中文字体,在容器里运行firefox 游览器,已经配置支付flash播放

## 用法

###运行容器

	docker run -d -P --name firefox lihaixin/firefox:s5

###修改VNC密码

	docker exec -it firefox /bin/sh -c "x11vnc -storepasswd VNCPASSWORD ~/.vnc/passwd"


###如何访问

	firefox http://<IP>:8787

	vncviewer <IP>:5900

