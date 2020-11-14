# YoCool-Console

适用于[HoshinoBot](https://github.com/Ice-Cirno/HoshinoBot)的插件，并且同时安装了插件版[yobot](https://github.com/pcrbot/yobot)，可以实现[YoCool](https://github.com/A-kirami/YoCool)主题的一键安装、升级、卸载等操作。


## 开始使用
本插件的安装方式与其他插件基本一致。

1. 下载项目，移动到`modules`目录下。
2. 在`__bot__.py`中添加本模块。


## 注意事项

1. 由于懒，直接使用了相对路径读写，请保证运行机器人主程序时，当前目录为`run.py`同级目录，例如：
   ```
   # 使用如下命令行运行时可正常
   python3 run.py

   # 不可, 当前目录不符合要求
   python3 /root/HoshinoBot/run.py
   ```

2. 安装与卸载时，由于移动文件和解压缩，会短时间内堵塞，约5~10秒，具体取决于您服务器的IO性能。
   
3. 使用了[fastgit](http://fastgit.org/)源来进行github的加速下载。您也可以自行修改第24行。