问题列表：

## 1
- 特征：不支持片选，即鼠标左键拖动可以区域选择文字进行复制、粘贴。无论是浏览器还是WPS，note中均常用到此功能。凤凰和remix两者以上功能均不可以
- 结果： 李兵组处理

## 2 Bug484
- 特征：浏览器，终端等不能使用快捷键，不方便使用。其他常用快捷键。凤凰和remix两者在电脑的浏览器中都可以使用快捷键，如截屏刷新等
- 结果：李兵组处理

## 3 BUG(493，494）
- 特征：桌面壁纸太丑，可以换一些壁纸。桌面右键更改壁纸，界面下方显示不完整，见附件。 桌面右键更改壁纸，界面显示比较慢，按esc退出后，显示黑屏，过很久才会回到桌面。 ；桌面图标乱序摆放，重启后该顺序没有了。凤凰和REMIX 全都没有这些问题，但是从体验上看，凤凰明显比REMIX更快，使用的流畅度更好。
- 结果：陈鹏处理

##4
- 特征：自带浏览器感觉很不舒服，体验不好。图片在浏览器上的显示效果太差 ；原生浏览器搜索视频播放，很多视频无法播放。原生浏览器在使用百度时，部分功能缺失，例如无法创建词条。 原生浏览器点击右上角选项的弹出框，点击弹出的设置选项，浏览器崩溃 ；Display contents in desktop mode. 凤凰和REMIX都安装不上firefox,凤凰内置星辰浏览器，remix内置谷歌。这两者在浏览图片的时候效果明显比我们好很多，星辰浏览器体验效果最佳，而且支持视频播放，但是播放的质量和体验都比较差，谷歌浏览器视频播放需要安装flash,目前没有发现又缺失的功能，但是我们内置的浏览器（不是firefox那个功能不全）我们的firefox浏览器，10月13号版本有严重的问题。
- 结果：陈刚+王之旭处理。建议自己编译源码来分析和改进

## 5 Bug501 
- 特征：从文件管理器往外拷贝东西太困难。凤凰没有识别，remix可以而且还支持ctrl+c  ctrl+v
- 结果：陈鹏 + 卢宁

## 6 Bug503 
- 特征：鼠标点击任务栏应用右键的选项时会触发桌面最大化窗口的应用。 凤凰和remiX不存在上诉问题
- 结果：董鹏组

## 7 Bug500 
- 特征：切换语言后，桌面右键仍然为开机时选择的语言。 凤凰和remiX不存在上诉问题
- 结果：王之旭？

## 8 Bug498 496 
- 特征：泰捷视频，打开后鼠标放在屏幕边界，可以更改窗口大小，无任务栏和窗口； 泰捷视频，终端等全屏应用打开后，按alt + f4关闭应用，任务栏消失。凤凰和remix在泰捷视频这方面均存在一点问题。窗口方面凤凰出现视频画面和窗口分离的问题，在视频加载阶段，remix是出现什么都没有直接回复到桌面，然后有几个加载的那个图标，过一短时间就成功进入画面（有点像WIN下网速不好，视频加载不上来的感觉）
- 结果： 李兵组处理

## 9 Bug473 
- 特征：Startmenu里，右键应用固定到任务栏功能缺失。凤凰和remiX两者均可以，不同的是remix是用左键，感觉remix体检更好。
- 结果：董鹏组处理

## 10 Bug476
- 特征：2016-10-19版本，无法从应用窗口的上边框改变窗口的大小。凤凰可以 remix不可以。
- 结果：王之旭

## 11 Bug475
- 特征：系统开机时间长，在openthos图标出现后，转约2分30秒左右的时间进入系统。缺对比！
- 结果：韩辉+王建兴

## 12 Bug470 469
- 特征：2016-10-19版本，在设置的wifi列表选择wifi，响应时间太久，要过一段时间才会连接上； 2016-10-19版本，点击右下角wifi列表会打开设置，但是wifi列表不消失。在wifi链接上两者全都么有问题，但是remix试用wifi比较慢
- 结果：李兵

## 13 Bug410
- 特征：2016-09-22 Firefox浏览器从常用界面 及常规打开网站时，底部显示异常，见附件。 凤凰和remiX两者安装多次firefox,均失败
- 结果：陈刚+卢宁

## 14 
- 特征：Window: Auto-hide and auto-show window title and statusbar.
- 结果：暂缓

## 15
- 特征：Google PinYin:Sometimes, it has no effect in QQ input content box, after restart QQ, it will be OK.这个问题两者目前没有发现，但是我们系统确实存在这样的问题
- 结果：暂缓

## 16 
- 特征：Startup Menu: Sometimes, the startup menu displaying is very slow, especially when IO is busy.
- 结果：董鹏改进， 韩辉+王建兴分析

## 17 
- 特征：电源问题：重启、睡眠及插拔电源时导致系统15秒休眠。
- 结果：陈刚

## 18
- 特征：U盘权限问题，文件管理器拷文件时会有权限问题。同一个U盘，只有remix可以用，同时支持快捷键，剪切复制
- 结果：王建兴
- 状态:已经处理完毕,还需要测试大量验证.

## 19
- 特征：机器放置一段时间会黑屏，且无法唤醒。凤凰和remix在首次开机不设置的情况下至少半个小时是没有问题的
- 结果：如果频繁出现，李兵组

## 20
- 特征：android studio 移植 到openthos上。
- 结果：陈刚

## 21 Bug488
- 特征：2016-10-20 小窗口显示的应用总是置顶，例如QQ、图库，当操作ES文件管理器等最大化窗口时，这些应用会遮挡弹出的信息。不频繁。
- 结果：

## 22 Bug472
- 特征：2016-10-19版本，英文模式下，开始菜单的右键菜单，显示不全，意义不明，见附件。-董鹏 
- 结果：暂缓

## 23 Bug486 
- 特征：QQ浏览图片没有放大功能。
- 结果：暂缓

## 24 Bug489
- 特征：2016-10-20 图库最大化窗口时，照片区域没有变化，右侧和下方为大片黑色区域，见附件。---需 自适应。remix没有专门的图库，凤凰的图库不存在这个问题
- 结果：暂缓

## 25 Bug487 
- 特征：途牛HD在窗口显示时 有文字重叠（显示金额和其它信息重叠，全屏没有此问题）
- 结果：暂缓

# 26
- 特征：在WPS Pro版中编辑文字时，方向键不能控制光标位置，只能通过鼠标定位。（remix,phoenix上试一下，看是否存在相同问题
- 结果：暂缓



#27 
- 特征：Ubuntu shell: Need a script to enter ubuntu command line directly. At present, the shell window size is not stable.
- 结果：暂缓

# 28
- 特征：谷歌输入法输入英文时两个单词之间自动填充空格，需手动删除。
- 结果：暂缓

# 29  Bug477
- 特征：2016-10-19版本，微信网页版无法打开，见附件，之前0905版本可以打开（浏览器问题，处于桌面模式 ）
- 结果：暂缓

# 30
- 特征：不支持2个或者2个以上QQ
- 结果：暂缓

# 31
- 特征：Games:Most of games are not supported.
- 结果：暂缓

# 32
- 特征：安装过于费劲，个人安装了差不多一个多小时，均失败，最后实在测试组的帮忙下，才安装成功（by王之旭）
- 结果：已解决 ，王建兴oto-ota 已有方法
