# clobotics——rootOnNVMe
0.备份镜像到指定目录
```
$ ./0_backup-rootfs.sh -d ddirectory
```


0.恢复镜像到ssd
```
$ ./1_copy-ssd.sh
```

2.设置启动
```
$ ./2_setup-service.sh
```

After setting up the service, reboot for the changes to take effect.


## Notes
* Initial Release, May 2020
* JetPack 4.4 DP
* Tested on Jetson Xavier NX


## 重新刷镜像步骤：
1.去掉ssd排线 

2.开机进入emmc系统，终端输入命令：sudo systemctl disable setssdroot.service  

3.关机插入ssd排线  

4.开机，格式化ssd，插入镜像硬盘  

5.进入镜像硬盘的BackAndRestore文件夹，运行 ./1_copy-ssd.sh

6.命令运行完之后，运行./2_setup-service.sh

7.重启
