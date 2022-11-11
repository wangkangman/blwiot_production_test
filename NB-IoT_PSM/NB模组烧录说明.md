<!--
 * @Author: Connor
 * @Date: 2022-11-11 14:48:16
 * @LastEditors: Connor
 * @LastEditTime: 2022-11-11 15:05:06
 * @FilePath: \碧林威生产测试文件\NB-IoT_PSM\NB模组烧录说明.md
 * @Description: 
 * 
 * Copyright (c) 2022 by Connor/BLW, All Rights Reserved. 
-->
# 模组俯视图
![a2d3092bb904198b9b17268ad581247.png](https://upload-images.jianshu.io/upload_images/27814183-16a1b7ecc9a14fdf.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 1. 为模组烧录固件。
### 1.1 串口烧录器，接“AT口/烧录口”，烧录器rx接模组tx，烧录器tx接模组rx，模组GPIO18接地。
![439093458ab4bd3e627b13870dd75a2.jpg](https://upload-images.jianshu.io/upload_images/27814183-22bc3ae9ce7f1762.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
### 1.2 解压缩ec616.rar，打开 ec616/FlashTools_V2.3.26/FlashTools.exe，选择串口烧录器对应串口号，其他内容按照图片设定。
![ad4263fe135d6019d0960a256a078e4.png](https://upload-images.jianshu.io/upload_images/27814183-b7466273629b1fb3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
### 1.3 上电，为模组烧录固件，烧录成功后信息栏会报成功信息。



## 2. 为模组重新授权SN码。
### 2.1 二、芯片授权，GPIO不接地，串口调试工具接“MCU通讯口”。



### 2.2 电脑安装涂鸦”生产解决方案”，进入安装目录。如 C:\Program Files (x86)\Tuya\TYProductionToolkit\tools\LittleOrange，Shift+鼠标右键，在此处打开Powershell窗口.
![image.png](https://upload-images.jianshu.io/upload_images/27814183-c0113165d745eb99.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 2.3 powerShell中输入 .\LittleOrange.exe ，启动授权程序。
![1667809174355.png](https://upload-images.jianshu.io/upload_images/27814183-c466c03fc12eb7e3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 2.4 右侧设置，选择本地导入。
![fa3af5753fcad596c22ea45c703fb74.png](https://upload-images.jianshu.io/upload_images/27814183-a62b23659c215abc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 2.5 按图中配置软件
![a0af2c720df549404231d10379f3f47.png](https://upload-images.jianshu.io/upload_images/27814183-63132a03e5cc7c09.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 2.6 勾选相关选项。
![5a144c8f19cb11f7b1ad28261291a6b.png](https://upload-images.jianshu.io/upload_images/27814183-f962b8f5b37d7638.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![bd4054294dadc38c82a8683408911cb.png](https://upload-images.jianshu.io/upload_images/27814183-1c5470b8103008b1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 2.7 点击红圈内设置按钮，设置接口信息（串口号依实际连接情况而定，波特率选择9600）。
![image.png](https://upload-images.jianshu.io/upload_images/27814183-1d1d0fbac8d7f367.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 2.8 输入新的SN码，然后先点击运行，然后为模组上电，测试成功后即完成授权。

