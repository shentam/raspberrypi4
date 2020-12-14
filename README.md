# raspberrypi4
setup
屏幕有黑边去除方法

/boot/config.txt 中修改第10行的：

Bash
nano /boot/config.txt


disable_overscan=0 //设置是否允许屏幕过扫描1为不允许，0为允许

Bash
reboot #重启系统


知识扩展：

overscan_left =16 //将画面向左移动16个像素点

overscan_right =16 //将画面向右移动16个像素点

overscan_top=16 //将画面向上移动16个像素点

overscan_bottom=16 //将画面向下移动16个像素点

disable_overscan=0 //设置是否允许屏幕过扫描1为不允许，0为允许

framebuffer_width=800 //设置屏幕宽度为800个像素点

framebuffer_height=400 //设置屏幕高度为400个像素点

Sdtv_mode=2 //设置树莓派输出的电视制式

0-NTSC，北美视频标准

1-NTSC-J，日本视频标准

2-PAL，英国和其他国家视频标准

3-PAL-M，巴西标准

sdtv_aspect=2 //设置输出画面宽高比，1-4:3，2-14:9，3-16:9





如果修改无效果，raspi-config➤➤Advanced Options➤➤Overscan，然后display
