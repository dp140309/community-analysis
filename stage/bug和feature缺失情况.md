# bug和feature缺失情况(修复时间：3.15~4.15 )
## 陈刚组：
### Firefox ：重要
- [bug]
1. [bug 893] 右侧菜单调一下，最长的菜单显示不全（提交时间2016-12-20 曹永韧  3.10）（曹永韧）
2. [bug 1140] 在浏览器中上传文件时会提示“摄像机、相机...“，选择相机会进入拍照界面，此时无法取消，点击右上角关闭相机界面则会将fennec一起关闭()，点击左上角回退不会关闭（刘晓旭）
3. [bug 925] Firefox 邮箱上下键不能用（搜索框中输入几个文字，如在下面弹出的猜测信息中含有自己需要内容，按方向的上下键无法选择对应输入信息）,ctrl+链接无法新建页 （陈刚）  
4. [bug 1221] fennec(20170405版)下载wandoujia apk，双击弹出安装对话框，关闭此对话框，整个fennec被关闭 （刘晓旭）
5. [bug 1182] 反复调整字体大小（设置-显示-字体大小 ），fennec最上方标准栏消失（超过屏外显示）（x） 
6. [bug 1198] fennec播放flash时，没有文字显示。（x）
- [feature]
1. 增强(E):浏览器增强（多实例，弹窗JS，右键，UI修改，PHONY+ublock origin预装配置）---陈刚
1. fennec应集成在system中，不可卸载------刘锋 (罗俊欢)
2. 请把这个addon(https://addons.mozilla.org/en-US/android/addon/ublock-origin/?src=search)作为默认项编译进fennec------刘锋（曹永韧）
3. 默认集成UA切换功能，或者phony扩展；默认集成ublock origin并订阅easylist china------刘锋 （曹永韧）
4. internet 浏览器预配置如下： a.安装扩展ublock origin和phony b. ublock默认启用 easylist china并更新列表 c.phony默认启用desktop firefox模式，并在用户手册中提示如果用户需要切换的话如何操作------刘锋 （曹永韧）
5. 设置-易用性-文本大小 默认改为“大”------刘锋 （曹永韧）
6. 设置最后一项“openthos”应该是Internet 浏览器(Internet Browser)------刘锋 （曹永韧）
7. 页面ctrl+滚轮放缩的缩放步进问题（10%步进？）------刘锋 （刘晓旭）
8. 搜索引擎默认为BING------刘锋（曹永韧）
9. 如果我们把user-agent切换的功能放到fennec里，似乎原生菜单上的“request desktop version”就没用了而且容易造成误解，建议删掉------刘锋（曹永韧）

### 多窗口问题：重要
1. 增强(E):  WM：横/竖屏，比例拉伸，预设配置，透明背景，菜单出屏，微信UI，office稳定性---陈刚，刘晓旭
1. [bug]弹出菜单在窗口外,共性问题。如：微信是右下角正常，其他位置均不正常（FM已修复，微信未修复）（陈鹏）
2. [feature]应用默认打开方式目前通过白名单启动，新安装其他应用默认均为手机模式。后期需完善。（刘晓旭，曹永韧）

### MS office 目前存在的问题：重要
1. [bug 1144] 大楼用户那里Excel闪退现象还是存在，并且即使手动保存一下闪退后鼠标所在单元格的数据就会消失，以至于用户在编辑完后赶紧把鼠标放到空白单元格处避免闪退后后原有数据丢失现象发生。（陈刚）
2. [bug 1066] msoffice word使用绘图功能时，使用橡皮擦功能会崩溃 （陈刚）
3. [bug 1191] 缺少关闭文档时的提示保存与否, 点击右上角关闭时，没提示是否保存，默认的是不保存。（曹永韧）
4. [bug 1023]excel调整比例100%后，保存关闭再次打开时仍为原大小，未保存设置(调研如何保存设置）-对比：手机上调整比例后再打开也会显示默认比例 (?陈刚)
5. _[bug 1068]excel中无法插入批注---------对比：手机上可以正常插入批注 （陈刚）----------------------------------已完成100%_ 


### WPS office
1. [bug 1163] wps-office通过qq进行分享时，关闭qq的同时也会关闭当前打开的文件（属于多窗口） (刘晓旭)
2. [bug 1190] 文档中内容不能按大小窗口比例缩放，点右上角“- 口x“ 这个标志，小窗口和最大话的对比，内容也应该按比例缩小，但是只是显示小窗口的大小，内容却是大窗口的比例。（陈刚）

### 微信
1. [bug 608] 升级之后消息，微信顶端会下沉（陈鹏） 
2. [bug 1046] 微信评论不支持表情符（2017-01-12发现）-之前功能是可用的，未定位从哪版开始失效 （陈鹏）
3. [bug 1048] 调整系统的音量不会改变提示音，系统声音（快捷调节音量部分）已经全部关闭了还会有提示声音（建议系统声音调节同时针对媒体音量、通知音量、闹钟音量）（曹永韧）

### QQ
1. [bug 824] 聊天消息无法复制粘帖-----------对比phoenix/remix的QQ，WECHAT复制粘贴情况 （卢宁）

|对比测试|phoenix|remix|openthos|
|------|------|------|------|
|QQ|1、聊天消息长按复制<br>2、输入框可选择文字，支持右键和快捷键进行复制粘贴|1、聊天消息长按复制<br>2、输入框可选择文字，支持右键和快捷键进行复制粘贴<br>3、输入框选中文字后自动弹出的菜单可以用，右键弹出的菜单有穿透效果，剪切无法使用|1、聊天消息长按复制<br>2、输入框需要长按才能选择文字，支持快捷键进行复制粘贴<br>3、聊天消息长按的弹出框位置偏移较大<br>4、输入框长按，在最上方会出现菜单|
|wechat|1、聊天消息长按复制<br>2、输入框可选择文字，支持右键和快捷键进行复制粘贴|1、聊天消息长按复制<br>2、输入框可选择文字，支持右键和快捷键进行复制粘贴|1、聊天消息长按复制<br>2、输入框可选择文字，支持快捷键进行复制粘贴<br>3、输入框长按，在最上方会出现菜单|

**总结：<br>1、聊天消息均只能长按复制，不能选择部分文字；<br>2、以上测试中，openthos的qq是应用商店中下载安装的，版本为6.3.7，若下载最新的6.7.0版本，则聊天消息无法复制；微信版本为6.3.18,与最新的6.5.6在复制粘贴情况上一致；<br>3、凤凰、技德均支持输入框中的右键菜单，openthos需长按显示菜单**


2. [bug 762] QQ，wechat来消息无提醒-  （？王之旭问刘明明）

`phoenix： 没有声音提醒，在右上方会弹出消息提醒，底部任务栏上的QQ图标会出现红色脚标数字1
 remix： 没有声音提醒，在右上方会弹出消息提醒。`
 
3. [bug 788] qq打开链接（总是在内部打开，不是外链）（？对比remix, huoji, x）  

`phoenix：打开链接时在内部打开。
 remix：打开链接时在内部打开。`

### 高德地图
1. [bug 1211] 高德地图白色背景变为透明，之前firefox进入全屏模式隐藏工具栏时也有类似情况 (卢宁)

## 王之旭组：
1. 工厂测试工具---王之旭
### File manager:重要
1. [bug 1131] 文件管理器点击卸载按钮，经常会使文件管理器崩溃退出，复现概率较高，非百分百。右键卸载不会出现此问题 （罗俊欢）
2. 压缩解压缩支持（建议直接出Application）（卢宁）
3. [feature]Auto Mount （王之旭）
4. [feature]文件管理器 向上功能 （陈鹏）
5. 调整字体大小（设置-显示-字体大小），名称显示不全。（周怡洁） 
6. 重命名时默认选中只含文件名，不含后辍。这样更符合用户使用习惯 （曾非非）

### 桌面：重要
1. [bug]1004 桌面-其它应用打开时无法重命名文件，且所有快捷键失效：F2、F5、ctrl + a、ctrl + c、ctrl+v、ctrl + x、ctrl+ 左键、Enter、delete、shift +delete (非100%复现) （刘晓旭）

### 应用商店（罗俊欢）
1. _[feature] 应用商店UI界面图标及进度条均显示过小（图标要大，跑马灯图片要高些），界面照抄playstore网页版即可 （UI出图研发改））_-------------------已完成100% _ 
2. [bug 1138] appstore首次打开时取缓存内容，不要直接显示最新而处于空白加载页面（提交时间2017-03-06 3.10 罗俊欢）
3. [bug 1043] QQ更新按钮可反复点击
4. [bug] 调节字体大小时会显示不全，需修复。


## 王建兴组：
### 安装：重要
1. 新增(+):系统部署工具（win->HDD）---王之旭，王建兴
2. 新增(+):BOTO->efi硬件，trusted boot支持---王建兴
3. 新增(+):预装软件，预配置镜像，磁盘分区方案，预载文档和壁纸---王之旭，王建兴，刘晓旭
4. 新增(+):kare lake(7 th core)gpu---王建兴
5. _增强(E): time与windows一致---王建兴-----------------------------------已完成100%_ 
6. 增强(E): FM，NTFS，AUTOMOUNT---王建兴，王之旭
7. 增强(E): GUI SLIENT BOOT---王建兴
1. [bug 1202] USER版本下 FM-只能看到安卓系统（1.9G 可用578M），硬盘空间大小只能在设置中看到。
2. [bug 504] 系统休眠一段时间，会出现不能唤醒，唤醒后卡死或者重启的现象，各设备复现率不一致，有的常现，有的偶现。(2016-10-25-王建兴)
3. u盘升级（4.15）


## 刘晓旭组：
### 谷歌输入法：重要
1. 桌面输入中文时与焦点依托--刘晓旭（×）
2. [bug 1217] 20170330版本，打开多个应用，互相切换，提示“谷歌输入法”停止运行，附log （！刘晓旭）

### 设置
1. _隐藏(H): 云同步功能（设置，FM隐藏）---刘晓旭，王之旭-----------已完成100%_  
2. _隐藏(H): firewall-刘晓旭-----------------------------------已完成100%_
1. ［feature］ 云服务布局不美观，间隔较大，优化;功能缺失，导出功能未实现； （李兵，刘晓旭 已完成壁纸，WIFI，浏览器，开始菜单,任务栏---剩应用数据）（x）
2. ［feature］ 应用默认启动方式-桌面/手机（目前通过白名单控制），修完善 （x）


## 曹永韧组：
### 通知栏
1. 增强(E): startmenu优化，状态栏配置保存---曹永韧
1. [bug 1048] 声音静音后微信声仍出声（曹永韧 2016－3－5后做）（曹永韧） 
2. [bug 1223] 点击格式化SD卡，openthos系统重启（？王之旭）-补充：`SanDisk黑色U盘（贴有win10标志）可复现此问题。`


### 任务栏
1. 任务栏显示/隐藏 状态重启后未保存（曹永韧）
1. 任务栏快速启动栏设置，重启后未保存（曹永韧）
1. [bug 1171] 如下图，截图时间为2017年03月08日，“8”被挤到了下一行，并且显示不全。这个问题在我这经常出现。系统版本：1.9.5(2017.03.06)硬件平台：清华同方（曹永韧）
1. [bug 1227] 窗口不会因为任务栏出现而自动上移，导致任务栏隐藏，鼠标移到最底下弹出然后最底下应用的按钮就按不到了。------社区（曹永韧）

### startmenu
1. 增强(E): 电源管理（sleep/wakeup ,wifi检测）---曹永韧，刘晓旭，王建兴
3. [bug 659] 打开游戏时，开始菜单打开时延迟---延后 （曹永韧）

### 关机界面：重要
1. [bug 016] 20160516版本-新增锁定-第一次要activate,步骤复杂。其它系统不允许此权限操作（曹永韧）
2. [bug 443] 睡眠首次会调超级用户权限.如图(修改睡眠回来四项仍显示出现的新问题)（曹永韧，王建兴）  
3. [bug 783] 重大锁屏BUG(不易复现)开机后不进行锁屏状态的解锁，待到系统熄屏，任意键唤醒系统，系统保持在熄屏状态，无法唤醒。（曹永韧，王建兴） 
4. [bug 1033] startmenu-电源-睡眠唤醒回到桌面后power菜单项会再次弹出在桌面上，且有时还伴有“系统界面“已停止的弹出框（曹永韧，王建兴） 
5. [bug 1110] 带密码的锁定-重启后进入锁屏界面，此时如不输入密码一会机器会自动进入睡眠状态，点击键盘上的enter或空格键唤醒，机器重启（T43U） <自动很快进入休眠状态是framework加的patch造成的,睡眠重启问题我会尽快复现-王建兴>（曹永韧，王建兴） 
 
### 第一次启动界面
1. [bug1120］ 首次配置时，本机设置页面直接按下一步，之后系统会无法重启  <刘晓旭调查出了原因,周怡洁在负责这个问题>（周怡洁）
2. [bug1200］ 首次配置时弹锁屏权限确认，导致无法输入字符（大家复现情况不同，我的电脑每次安装都会出现此问题，张琳萍的有时会出现，概率大概70％-80％） <这个是315前两天加的patch造成的,曹永韧在负责这个问题>（曹永韧）

