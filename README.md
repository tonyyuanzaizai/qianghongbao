# qianghongbao

资料：
http://blog.csdn.net/feifei454498130/article/details/43891781/
https://github.com/lendylongli/qianghongbao
原作者：
个人博客:http://www.happycodeboy.com
Email:codeboy2013@gmail.com
QQ:730395591

研究安卓app自动化测试
此次仅仅用最新的androidstudio 编译打包，做调试备份。

环境准备：
1. 下载最新版androidstudio
2. 始终开启vpn
3. gradle 版本要使用对应版本，这个是用的4.5


IDEA切换到DDMS视图 Tools-Android-Android Device Monitor

关闭360

夜神模拟器
http://blog.csdn.net/feifan_feimeng/article/details/57415278

AndroidStdio打开DDMS方式：Tools——>Android——>android devices monitor. 
问题：若打开DDMS后没有显示连接的device。 
解决办法： 
①先启动夜神模拟器

②然后运行cmd命令，cd到夜神安装目录（bin文件夹下），执行命令nox_adb.exe connect 127.0.0.1:62001

或直接打开夜神模拟器安装目录（bin文件夹），然后在地址栏输入adb回车，再执行命令nox_adb.exe connect 127.0.0.1:62001

或将夜神模拟器安装目录（bin文件夹）路径，配置在环境变量path中，直接执行cmd命令nox_adb.exe connect 127.0.0.1:620010

即可连接到模拟器

③如果无法看到夜神模拟器，请adb后，重新启动下夜神模拟器

④注意：不要开启其他模拟器，因为夜神模拟器与其他模拟器不兼容（开启多个不同种类模拟器，会同时开启多个adb.exe进程，而系统只能识别一个adb.exe进行）