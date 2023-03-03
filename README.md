# PlayWithTello
创建这个项目仅仅出于娱乐目的。目前可以用键盘控制Tello，可以视频图像，有些功能还未完成（利用姿势控制等）。
代码中注释较多，且没时间写文档，大家见谅。   
TelloController是主类，可以直接运行。    
姿势识别部分试用了一下mediapipe，感觉挺强大的，以后有时间在继续维护吧：）

使用的库：   
Python 3.7.3   
keyboard：0.13.5   
numpy：1.21.6
opencn-contrib-python：4.7.0.72     
mediapipe：0.9.0.1 


安装opencv及mediapipe：  
安装的先决条件： numpy>=1.17.0; python_version >= "3.7"   
1）升级pip到最新版本，这里用的版本是23.0.1  
2）使用命令再次升级pip（可能是让pip支持wheel的）：pip install --upgrade pip setuptools wheel  
3）使用下面两个命令以此安装opencv及mediapipe  
（1）pip install opencv-contrib-python -i https://pypi.tuna.tsinghua.edu.cn/simple  
（2）pip install mediapipe -i https://pypi.tuna.tsinghua.edu.cn/simple     
安装后的版本为：   
opencn-contrib-python：4.7.0.72     
mediapipe：0.9.0.1    
在这个过程中，PIP似乎会自动安装相关依赖包。


mediapipe安装与使用，参考：https://blog.csdn.net/m0_52364694/article/details/120825352    

opencv-python 是只包含了主要模块的包，opencv-contrib-python包含了主要模块以及扩展模块，扩展模块主要是包含了一些带专利的收费算法（如shift特征检测）以及一些在测试的新的算法（稳定后会合并到主要模块）。

MediaPipe介绍参考：https://blog.csdn.net/weixin_38346042/article/details/123399492。   
注意这个库要依赖OpenCV来处理视频，FFMPEG来处理音频数据。它还有其他依赖项，如OpenGL/Metal、Tensorflow、Eigen等。