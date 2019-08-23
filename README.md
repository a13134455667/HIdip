#简单开启HIDIP

##获取显示器ID
在终端中输入下面命令
`ioreg -l | grep DisplayVendorID`

就可以可以看到DisplayVendorID (显示器制造商ID)
如 ”DisplayVendorID" = 16652

然后，在终端中输入下面命令
`ioreg -l | grep DisplayProductID`

就可以看到DisplayProductID (显示器产品ID)
如 "DisplayProductID" = 49297

这两个数字都是十进制的，用计算器功能或在线转换把它们换算成16进制。
以上面为例
`16652 ==> 410c`
`49297 ==> c091`


文件夹名就改为 DisplayVendorID-410c
文件名就改为 DisplayProductID-c091
然后把修改好的文件夹放入目录：
`/System/Library/Displays/Contents/Resources/Overrides/`
