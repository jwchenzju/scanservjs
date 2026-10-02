# scanservjs
基于 sbs20/scanservjs，增加了HP MFP 1188的扫描驱动
https://hub.docker.com/r/jwchenzju/sane-web

#基于 sbs20/scanservjs，增加了HP MFP 1188的扫描驱动 docker run
-d
--restart unless-stopped
--log-driver local
-p 8080:8080
--device=/dev/bus/usb:/dev/bus/usb
--name sane
jwchenzju/sane-web:1.0

化工农民折腾的镜像，不严谨，玩玩就好。不要扫描和打印同时挂USB使用，会打印乱码的。

