# freeRealtimeTranslation
free realtime translate tool

### 项目介绍(description)
免费的实时系统声音翻译工具,包含了系统声音录制，实时语音识别，翻译功能  
Free real-time translate tool for system audio,inclding system audio recording,automatic speech recognition,and translate

可以用来在英文电话会议(比如面试),或者听无字幕视频的时候实时生成双语字幕  
Can be used to generate subtitles during telephone conference calls (such as ZOOM/Webex), or when listening to unsubtitled videos

默认支持英文转中文,你可以下载其他语音包支持其他语言   
Default convert from English to Chinese,but you can change it to your language  

支持其他语音的办法：  
在 https://alphacephei.com/vosk/models 下载语言包，然后替换原来的model文件，或者新建一个model文件夹，比如model-cn，将main.py中的model改为新的文件夹路径。  
另外需要修改开头的settings中的API域名和语言代码。  
Ways to support other languages:  
Download the language pack at https://alphacephei.com/vosk/models, then replace the original model file, or create a new model folder, such as model-cn, and change the model in main.py to the new folder path.  
And you also need to modify settings in the main.py.




### 安装 (install)

#### pip安装依赖（pip install dependency）：  
googletrans==3.1.0a0  
vosk==0.3.32  
sounddevice==0.4.4  
numpy==1.19.5  
scipy==1.6.0  

#### 系统环境 （system envirnmont）
在mac上安装  
需要安装blackhole虚拟声卡用来录制，  
搜索midi设置,新增一个多输出设备，选择blackhole和你的耳机或者扬声器。  
这样声音就会既被你听到，又被blackhole转成了一个输出。增加完之后需要右键将这个设备设置成输出设备。

install on mac  
Need to install blackhole virtual sound card for recording.  
search for midi settings,add a multi-output device, choose the blackhole and your headphones or speakers. This way the sound will be both heard by you and converted into an output by blackhole. After adding, you need to right-click to set this device as an output device.

have not test on windows yet.

### 运行(run)
运行main.py
run the main.py

### 作者邮箱：  
author email:  
meng93914@gmail.com

csdn文章地址： https://blog.csdn.net/Memory_and_Dream/article/details/123199398
欢迎直接留言咨询
