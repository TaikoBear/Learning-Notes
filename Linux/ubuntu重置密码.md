> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [blog.csdn.net](https://blog.csdn.net/yaotai8135/article/details/100084584)

很多使用 ubuntu 的小伙伴可能会想要修改自己的用户名。在修改用户名过程中，如果你没有切换到 root 权限，而只是执行 sudo vim /etc/passwd，那么在修改了 / etc/passwd 这个文件中的用户名部分、用户组部分和主目录部分之后，如果你退出了，那么修改了用户名之后与密码无法匹配，退出系统更是再也登录不上，也无法切换到 root 权限。  
针对这一问题，有人说要重装系统，其实不需要，现给出解决办法如下：

1.  重启电脑，进入 grub 启动菜单（开机时长按 shift 键或 Esc 键，注意：可能不是所有同学的电脑都适用上述快捷键，如果上述按键进入不了 grub 菜单，可以尝试一下 Ctrl+Shift+F1）;
> Type **normal**, hit Enter, and then tap **Esc** until the menu is displayed. Hitting **Esc** at this point won't drop you to the grub command prompt (so don't worry about hitting Esc too many times).

2.  进入 grub 菜单模式找到 Ubuntu 高级选项并进入 recovery mode 选项，(注意：部分电脑可能会直接进入 grub 命令行，在命令行输入 normal 可以直接进入 grub 菜单模式)。里面可能有多个 recovery mode，选择第一个，按 e 进入编辑模式，找到命令中的 recovery nomodeset 修改为 quietsplash rw init=/bin/bash

3.  按 F10 进入命令行模式， 输入 mount -rw -o remount / 获得读写权限;

4.  输入 vi etc/passwd 打开需要修改的文件, 将用户名修改为原来的用户名;

5.  按照 vi 编辑器的规则修改好内容后 Ctrl+Alt+del 重启即可恢复正常。