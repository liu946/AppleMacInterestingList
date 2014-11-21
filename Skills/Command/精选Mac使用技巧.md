## 学习了：精选Mac使用技巧，很实用哦
【转】http://www.douban.com/group/topic/17257981/
<pre>
学习了：精选Mac使用技巧，很实用哦 
2D/3D Dock 切换 
在Terminal（命令行窗口）中输入如下命令进行切换 
defaults write com.apple.dock no-glass -boolean YES; killall Dock 
defaults write com.apple.dock no-glass -boolean NO; killall Dock 
预览时删除图片 

使用Preview查看图片时，使用command + delete可直接删除该图片。 
一次性下载多个文件 

在safari中，command + option + L 打开下载窗口，再command + V粘贴多个链接即可。 
慢动作 

加上Shift键, 很多效果都会是慢动作. 包括Stack、Exposé、窗口变换等等. 
查看多个文件的Info 

如果需要查看2个或更多文件的Info, Command+I会为每个文件打开一个Info窗口。如果有几十个文件，想看到文件总大小等info信息，可以使用Option+Command+I打开，这样只会开启一个Info窗口（该窗口将显示这批文件汇总的信息）。 
Spaces间拖动同一程序的多个窗口 

在从一个空间把程序拉到另一个空间的时候按下Shift可以把所有同样的程序一起拉. (例如好几个Safari窗口) 
快速进入幻灯片 

选择多图然后按Option+Command+Y可以让你进入全屏幻灯片.当然, 一张图也可以. 
转换DMG到ISO格式 

在命令行窗口运行： 
hdiutil convert filename.dmg -format UDTO -o outputfile.iso 
使用Finder登录FTP 

打开Finder然后按Command+K，输入服务器信息、用户名与密码，即可连接上FTP服务器。 
预览时对图片进行标记 

使用Mac系统默认的图片预览工具Preview即可对图片进行标记，Ctrl + Command + O可画出椭圆，Ctrl + Command + T可书写文字。 
快速使用Google搜索 

只要是Cocoa程序, 你都可以选择一些文字然后按Shift+Command+L快速以Google搜索。（在Safari中试试看） 
快速关闭屏幕 

按shift+control+eject(退盘键) 可以把屏幕立即关掉，按任意键唤醒。 
取消抓图时的阴影 

当你使用Shift + Command + 4然后放手再按空格抓一个窗口的时候, 窗口是有投影的.如果需要可以取消投影，请在命令行窗口输入如下代码： 
defaults write com.apple.screencapture disable-shadow -bool true 
需要显示阴影： 
defaults write com.apple.screencapture disable-shadow -bool false 
回收站的文件删不掉怎么办 

有时候我们在清除Trash的时候系统会提示说某些文件被使用无法删除，通常是指该文件在使用之中。此时，打开命令行窗口Terminal，输入lsof 文件名（也可直接拖动文件到命令行窗口中），即可查看是哪个程序在使用这个文件，将对应程序关闭掉后，即可删除了。 
lsof /Users/devon/Desktop/demo.tif 
Safari在新标签页中打开搜索内容 

无论在地址栏或者搜索栏输入，只要按conmmand+enter就可以在新标签页打开。 
文字编辑时的光标移动 

Ctrl + p 上一行 
Ctrl + n 下一行 
Ctrl + f 下一个字符 
Ctrl + b 前一个字符 
Ctrl + a 行首 
Ctrl + e 行尾 
清除DNS缓存 

10.5.x: 
dscacheutil -flushcache 

10.4.x: 
lookupd -flushcache 
删除Safari 4 的 Top Sites 缓存 

Safari的Top Sites缓存下都是图片，通常会有几百M甚至上G，如果不用Top Sites，可将该文件夹设为Lock，这样就不会写文件进去了。如果设Lock：在目录上用Command + I打开Info窗口，在里面有Lock的选项。 
微调音量 

shift＋alt＋音量调控键，可微调音量。 
Safari 前进后退快捷方式 

safari前进或后退另外一种方法：三个手指在触摸板上左右滑即可（与图片翻页一样操作）。或者，直接按左右方向键可以翻到下页或前页。 
下载网络视频 

在上视频网站里，如果想将其flv的视频下载回来，用Safari就可以做到啦。在播放视频的页面，使用⌘+option+a，打开activity window，在里面可找到文件尺寸很大的以flv结尾的文件，这就是下载路径啦。 
快速退出移动硬盘 

Command＋E 可以快速退出移动硬盘。 
同一程序的多个窗口间快速切换 

cmd＋·，就是tab上面“～”的这个键！ 
在safari中使用reader功能 

Shift + Command + R，可打开查看网页时的Reader功能（部分网页支持）。 
忘记系统密码怎么办 

方法一：找出电脑原配的系统盘，重新启动电脑（电脑启动的时候按C键），选好语言后进入安装的时候，点击“常用工具”，里面会有一项是“重设密码”，这时你就可以重新设定系统的管理员密码了。 

方法二：开机， 启动时按“cmd+S”。这时，你会进入Single User Model，出现像DOS一样的提示符 #root>。请在#root>下 输入 (注意空格, 大小写) 
fsck -y 
mount -uaw / 
rm /var/db/.AppleSetupDone 
reboot 
紧接着，苹果电脑会重启 ，并且在开机后出现新装机时的欢迎界面。你需要像第一次打开苹果电脑一样， 重新建立一个新的管理员账号（数据会保留）。当开机完毕之后，在新的管理员下请打开 系统预制 － 账户。打开最下面的锁， 当跳出密码框时， 输入新的管理员帐号密码。这时，你会看到出现至少两个账号，包括了新的管理员的帐号和你原来的帐号。你可以点中原来的账号, 选 密码 － 更改密码。注意，你不需要有原先的密码就直接可以设定新密码了。下一步就是点下面的登陆选项 (小房子)。选中自动以右边的身份登陆， 同时在下拉菜单中选你原先的账号。当重启或注销之后，你可以用新密码登陆原帐户了。当然，你也可以将刚刚新建的帐户删除