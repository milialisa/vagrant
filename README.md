## 虚拟机开发环境

> 主要是为了简化配置开发本地环境

安装VirtualBox
```
https://www.virtualbox.org/
```

安装Vagrant
```
https://www.vagrantup.com/
```

下载box
```

```

xshell
```
Windows 安装个 xshell
Mac 不用
```

正式开始进行操作~
```
1. 新建一个文件夹作为工作目录

2. 打开一个dos窗口，初始化该目录，然后导入box
    vagrant init
    vagrant box add icolumn {url}

    Note: 导入box的默认指令
    vagrant box add {name} {uri}
    {name} 随意
    {uri} 就是你下载的 box 的路径(这里可以直接用 box 的在线地址, 但是这样太慢, 就选择下载下来直接用)
```

mac 上有 bug, Vagrantfile missing
```
Work-around

Unpackage box tar xvfz package.box <workdir>.
Manually add customized file cp Vagrantfile <workdir>/
Package box tar cvfz package.box <workdir>

```