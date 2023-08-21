# SSH

##  Windows 11 $\to$ Windows 10
  - [Windows10 openSSH](https://blog.csdn.net/weixin_43064185/article/details/90080815)


# Latex 

## [install](https://blog.csdn.net/zhu_rui/article/details/124551516)


# Linux 子系统

## [WSL2出现“参考的对象类型不支持尝试的操作”的解决方法](https://www.jianshu.com/p/7bd8cfbb5b01)

- 1. 临时方法(netsh winsock reset)
- 2. 永久方法
    - 下载工具至c盘（http://file2.happyjava.cn/NoLsp.exe）
    - .\NoLsp.exe C:\windows\system32\wsl.exe
## [WSL迁移](https://blog.csdn.net/qq_43557907/article/details/124737472)

- 查看安装的WSL版本
  - wsl --list
- 打开PowerShell，终止正在运行的分发或虚拟机：
  - wsl --shutdown
- 对需要迁移的分发或虚拟机导出（我安装的版本是Ubuntu-20.04）：
  - wsl --export Ubuntu-20.04 D:\wsl-Ubuntu-20.04
- 卸载分发版或虚拟机
  - wsl --unregister Ubuntu-20.04
- 导入新的分发版或虚拟机（“新的安装路径”这几个字不能删）：
  - wsl --import Ubuntu-20.04 新的安装路径 D:\wsl-Ubuntu-20.04 --version 2
- 接下来需要找回一下账户：
  - ubuntu2004 config --default-user 用户名（huanghao）
