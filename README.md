# 弹簧质点系统
## 项目背景
从taichi编程语言的爆红了解到了胡渊明大神，从他在bilibili发布的视频教程我了解到了弹簧质点系统的模拟，并尝试用C语言和easyx图形库实现相关功能，不仅如此，我还开发出了自己的独特功能，比如用颜色来表示力的大小。后来靠它完成了C语言大作业，并且得了A的好成绩。之后我会继续完善，现开放源代码供大家交流学习。
## 安装
 - 操作系统：Windows XP(sp3) 及以上操作系统。
 - 编译环境：Visual C++ 6.0，Visual Studio 2008 ~ 2019 (x86 & x64)。
本程序仅有一个文件，但由于其引用了easyx.h，所以不支持gcc编译器。下载之后，打开vs，将其添加到项目中，生成项目即可完成编译。
## 使用
1. 点击鼠标左键，就会在窗口里鼠标指针的位置生成一个质点，该质点的速度和位移受重力，空气阻力，以及可能的弹簧力和减震阻力的影响。质点会受重力下落，但不会超过窗口区域，会被限制在窗口区域内。当鼠标指针位置与其他质点的距离小于一定值时，指针与这些质点间会产生一条辅助线，点击鼠标左键将会生成一个与这些质点相连的新质点，它们之间的线就是弹簧，该弹簧符合胡克定律，但弹簧两端的质点会受到减震阻力，因而整个系统会逐渐静止下来。
2. 点击鼠标左键+ctrl键，会在窗口里鼠标指针的位置生成一个红色的、固定在空中的质点，该质点除了速度永远为零外与其他质点的物理性质完全相同。
3. 按下鼠标右键会在鼠标指针处生成一个引力点，可以吸引所有的质点聚集于此。
4. 按下鼠标右键+ctrl键，暂停更新所有质点的大多数数据，此时看上去他们就会被定在空中，但是此时仍可以生成新质点，也可以连接新弹簧。
5. 点击鼠标中键，撤销上一个质点的生成。
6. 点击鼠标中键+ctrl，清空质点和弹簧。
7. 按下鼠标右键+shift键，开启或关闭受力示意功能。开启后，弹簧颜色越接近绿色，弹簧力越小；颜色越接近红色，弹簧力越大。
8. 按下ctrl键再滚动滚轮，即可调节弹簧的劲度系数值，初始值为10。
9. 按下shift键再滚动滚轮，分两种情况：如果此时鼠标指针在窗口左半部分，那么就可以调节空气阻力系数；否则可以调节减震系数。
10. 屏幕上会显示使用信息，以及五个重要数据（当前质点数、当前弹簧数、当前劲度系数、当前空气阻力系数、当前减震系数）的实时值。
11. 屏幕右上角还会显示FPS值，也就是每秒显式循环次数。
## 参与贡献方式
使用项目的Issues功能，但可惜我平时不常来看，或者使用其他方式联系我。
看到这个项目的人估计都是我认识的人，直接用QQ或者微信联系我即可。
