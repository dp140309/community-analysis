### 简介

本文件记录Openthos8.1各个版本的更新情况

下载位置：

- 清华大学开源软件镜像站
- 百度网盘：提取码unx6
- fosshub

### 详情

#### 20191102版本(包含20180811~20191102patch)

##### 新增功能

- 新增虚拟权限管理
- 新增手机模式
- 安装完毕后，新增了调试选项，方便对系统错误进行调试。
- 新增虚拟wifi的功能，当app要求必须使用wifi环境才能使用时可使用此功能。

##### 修复问题

- 修复USB启动的问题
- 合并AOSP最新的代码
- 优化了Openthos8.1的启动速度和启动的稳定性
- 解决了一台电脑上多个Openthos系统不能共存的问题
- 解决蓝牙不能使用的问题

##### Change log

1. Add virtual permission management
2. Add compatible mode
3. Add function : virtual wifi
4. Repair usb boot
5. Getting startup time quicker
6. Multiple Openthos installation on one computer
7. Repair that the Bluetooth is not available

#### 20180811版本(包含0810patch）

##### 修复问题

 - 解决ssh、scp的segmentation fault
