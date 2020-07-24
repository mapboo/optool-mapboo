# optool-mapboo

本项目是整合 optool:https://github.com/alexzielenski/optool.git 将原有项目中添加了ArgumentParser内容，无需多次下载编译，运行项目即可编译出optool。

使用步骤：

1，git clone https://github.com/mapboo/optool-mapboo.git

2，运行项目编译出optool

3，将optool移动到/usr/local/bin目录下，终端打开：open /usr/local/bin

4，简单命令示例：

    A）注入动态库：optool install -c load -p "@executable_path/Frameworks/xxx.dylib" -t yyy
    
    B）删除动态库：optool uninstall -p "@executable_path/Frameworks/xxx.dylib" -t yyy
    
        注意：  xxx 表示动态库名称，Frameworks/xxx为动态库路径；
        
                yyy 表示Mach-O二进制文件；
