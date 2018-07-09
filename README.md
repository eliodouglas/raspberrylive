# raspberrylive
A tool which can play videos on Live site by raspberry

一个树莓派用的直播工具
同样适用x86的windows和linux平台
鉴于斗鱼b站等直播网站经常改推流码，每次重写脚本很烦。所以做个小工具

推荐树莓派系统是raspbian stretch 即debian 9 这个系统的软件源很多软件是比较新的，省去很多麻烦
如果是debian 8 系统 请看wiki手动编译暗转ffmpeg方法

首先安装ffmpeg
sudo apt install ffmpeg

安装qt（如果需要）
sudo apt install qt5-default qtcreator

下载源代码
git clone https://github.com/suntaobuaa/raspberrylive

cd /raspberrylive

qmake

make
即可

或者用qtcreator打开.pro.user 文件  编译运行

目前支持两个模式，电影模式支持推流时添加字幕，但是树莓派性能不够，必须在x86平台运行

电视剧模式，自动顺序播放文件夹下所有视频文件，不支持字幕功能，如需字幕，必须视频自带硬字幕

未来考虑添加批量烧写字幕功能







