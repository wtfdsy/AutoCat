[码云](https://gitee.com/youyi_sizruru/AutoCat)

## 警告

运行前，最好把一些小游戏先点掉（例如喂小鸡，淘宝人生等等），该脚本无法识别这些。

本项目的所有脚本以及软件仅用于个人学习开发测试,勿用于商业及非法用途，如产生法律纠纷与本人无关。

## 环境

python 3.3以上(最好是3.8), 64位

依赖安装：pip install -r requirement.txt

因为用到PaddleOCR识别文字，配置比较麻烦

[最好参考PaddleOCR官方推荐来安装python](https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.4/doc/doc_ch/environment.md)

可能还需要安装Microsoft C++ Build Tools和windows sdk，最好使用Visual Studio Installer来安装

<u>运行时会下载文字识别的模型，请保持网络畅通。</u>

airtest>=1.12.3 修改的获取屏幕截图的方式，运行过程中可能需要安装yosemite的应用

## 运行

python auto.py [--device/-d device_name]

device_name 可以通过 adb devices 命令来获取，默认取第一个设备

在android手机上开启USB调试和模拟点击.

然后运行脚本，脚本会自动运行进入活动做任务，如果开始运行时，你前台应用是支持的APP中的一个，则该脚本只会做该APP的任务，否则会做所有支持的APP的任务。

支持的APP：淘宝，京东，京东金融，支付宝。

支持的活动：618，双11等类似喵币的活动。

~~本人会在活动出来时候尽可能早点做适配。~~




