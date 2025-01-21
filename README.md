**WHAT IS THIS  这是什么**

This is a small hack that let Qt defaultly support decimal scale factor. After using it, you should use Fusion style and should not use QGraphicsEffect, or bugs will occur. Currently, this hack supports Qt **5.6** (**MinGW** release).  
这是一个让 Qt 默认支持小数缩放因子的小工具。使用它后，您应使用 Fusion 风格，不应使用 QGraphicsEffect，否则会出现错误。目前，此工具支持 Qt **5.6**（**MinGW** 版本）。

**HOW TO USE  如何使用**

Open C:\Qt\Qt(version)\(version)\mingw(version)\plugins\platforms, replace qwindows.dll and qwindowsd.dll.  
打开 C:\Qt\Qt(版本)\(版本)\mingw(版本)\plugins\platforms，替换 qwindows.dll 和 qwindowsd.dll。

**HOW TO COMPILE  如何编译**

Open C:\Qt\Qt(version)\(version)\Src\qtbase\src\plugins\platforms\windows\qwindowsscreen.cpp, delete "qRound" in QWindowsScreen::pixelDensity, save file, recompile Qt, get qwindows.dll and qwindowsd.dll.  
打开 C:\Qt\Qt(版本)\(版本)\Src\qtbase\src\plugins\platforms\windows\qwindowsscreen.cpp，删除QWindowsScreen::pixelDensity中的“qRound”，保存文件，重新编译Qt，获得 qwindows.dll 和 qwindowsd.dll。
