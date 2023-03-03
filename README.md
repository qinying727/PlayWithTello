# PlayWithTello
创建这个项目仅仅出于娱乐目的。目前可以用键盘控制Tello，可以视频图像，有些功能还未完成（利用姿势控制等）。
代码中注释较多，且没时间写文档，大家见谅。   
TelloController是主类，可以直接运行。    
姿势识别部分试用了一下mediapipe，感觉挺强大的，以后有时间在继续维护吧：）

使用的库：   
Python 3.7.3   
keyboard：0.13.5   
numpy：1.21.6

安装opencv及mediapipe：    
mediapipe安装与使用，参考：https://blog.csdn.net/m0_52364694/article/details/120825352    
安装的先决条件： numpy>=1.17.0; python_version >= "3.7" 

使用下面两行命令：   
pip install opencv-contrib-python -i https://pypi.tuna.tsinghua.edu.cn/simple    
pip install mediapipe -i https://pypi.tuna.tsinghua.edu.cn/simple

MediaPipe介绍参考：https://blog.csdn.net/weixin_38346042/article/details/123399492。   
注意这个库要依赖OpenCV来处理视频，FFMPEG来处理音频数据。它还有其他依赖项，如OpenGL/Metal、Tensorflow、Eigen等。