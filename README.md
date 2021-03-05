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

