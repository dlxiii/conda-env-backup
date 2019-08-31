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