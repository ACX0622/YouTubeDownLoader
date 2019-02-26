# Youtube Download

红石科技搬运组工具软件，用于自动下载视频，视频封面，字幕，同时规范简介格式。      
搬运组空间：[https://space.bilibili.com/1311124](https://space.bilibili.com/1311124)      
作者：Aye10032 [https://space.bilibili.com/40077740](https://space.bilibili.com/40077740)     

## 依赖环境

Windows系统；      
[python3](https://www.python.org/downloads/);     
代理软件;        

## 使用方法

首次运行先运行buildEnvironment.bat，自动配置环境，或者你也可以选择自行配置环境：
```batch
pip install pyperclip requests youtube_dl
pip install -U wxPython

# 之后再将本文件夹中的res文件夹加入系统环境变量的path变量中即可
```

正常运行直接双击运行run.bat即可

## 界面设置

设置搬运者ID，是否适用代理（如果代理是部署在路由器上选择不使用即可），以及代理IP，**代理必须是以http：//开头**，之后跟上IP及端口号即可。
这里编辑完毕后点击保存下次运行软件时会自动载入配置。

输入视频链接，点击下载按钮即可开始。运行结束后可以点击按钮复制简介部分的文字。     
你也可以仅点击**获取简介**按钮来仅获取简介信息而并不下载视频；       

对于自定义视频质量功能，在勾选该复选框并输入视频链接后，点击边上的搜索按钮获取视频可用格式列表，点击你要的音频及视频格式并关闭该窗口，之后点击**加载**按钮，文本框显示你选择的视频格式代码。如果想要修改格式重复上述动作即可。选择好格式之后点击下载视频按钮即可。     
如果你得电脑上装了ffmpeg程序会自动调用，没装会用默认方法合成音频及视频，但实际上也就慢一点点。