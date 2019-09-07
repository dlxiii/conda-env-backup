# conda env backup
 
导出已有环境：

~~~bash
conda env export > environment.yaml 
~~~

环境会被保存在 environment.yaml文件中。 
当我们想再次创建该环境，或根据别人提供的.yaml文件复现环境时，可以：

~~~bash
conda env create -f environment.yaml
~~~

就可以复现安装环境。
————————————————
版权声明：本文为CSDN博主「vola9527」的原创文章，遵循 CC 4.0 BY-SA 版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/vola9527/article/details/80744540

就可以复现安装环境。移植过来的环境只是安装了你原来环境里用conda install等命令直接安装的包，你用pip之类装的东西没有移植过来，需要你重新安装。

pip导出安装的库到requirements.txt

~~~bash
pip freeze > requirements.txt
~~~

pip导入requirements.txt中列出的库到系统

~~~bash
pip install -r requirements.txt
~~~

作者：宇果_2fdc
链接：https://www.jianshu.com/p/b86c17057da8
来源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。

查看当前包 

~~~bash
python -m pip list 
~~~

备份环境 

~~~bash
python -m pip freeze > /Desktop/myrequirements.txt 
~~~

安装环境 

~~~bash
pip install -r /Desktop/myrequirements.txt
~~~

来源：https://blog.csdn.net/lazybones_3/article/details/79504035

安装PYFVCOM错误解决：
* 参照：https://stackoverflow.com/questions/57243141/error-command-errored-out-with-exit-status-1-while-installing-requirements
* 参照：https://stackoverflow.com/questions/55084003/pyproj-package-installation-proj-dir-variable
* 参照：https://github.com/pyproj4/pyproj/issues/227
