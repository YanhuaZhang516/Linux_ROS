# Linux

## .bashrc
Bash is a pre-installed shell on the Linux distros.`.bashrc` 每次打开新终端的时，都会被读取。修改.bashrc可以改变环境变量PATH,别名alias 和提示符。

1. check the hidden files
```
ls -a
```

2. how to open .bashrc file?
```
gedit .bashrc
```
3. how to edit PATH?

PATH变量决定了shell将在哪些目录中寻找命令或程序。如果要执行的命令的目录在$PATH中，就不必输入这个命令的完整路径，直接输入命令就可以了。
三种方法修改环境变量：
- 直接用export命令
```
#export PATH=$PATH:/home/.../bin
```
查看是否设好可以用命令`export`查看

- 修改profile或者.bashrc文件(需要重启)

```
export PATH="$PATH:/home/.../bin"
```
4. What dose `source` mean?

`source` 是一个 bash shell 在现有(current)的shell里执行文件

```
> type source
source is a shell builtin
```
在ROS中创建了workspace后，需要将workspace中的setup.bash文件写入 ~/.bashrc 文件中，让其启动：
```
source /opt/ros/melodic/setup.bash
```
即开启新的terminal时候，运行这个setup.bash，这个setup.bash可以让一些ROS* 开头命令使用。同时创建一些ROS开头的环境变量。


