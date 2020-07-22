## Ubuntu | 分区

efi: 逻辑分区 200MB 用于Ext4，挂载点为“ /boot”

SWAP: 物理内存2倍 16*1024=16384MB 用于 Swap Area

/: 这是ubuntu 的根目录,用于安装系统和软件，相当于windows的C盘，一般100G，主分区，空间起始位置，用于"ext4日志文件系统"，挂载点为"/"

/home:相当于windows的其他盘，剩下的全分给它，逻辑分区，空间起始位置，用于"ext4日志文件系统"，挂载点为"/home"

## Ubuntu | 装机软件

- [Ubuntu 18.4 解决apt-get 下载速度太慢的问题](https://blog.csdn.net/Nonpc123/article/details/90050763)

打开Sofware & Updates

下载自

Others

select best server

close

reload

- ubuntu18.04 无线网络网速慢的解决方法

  ```shell
  sudo lshw -numeric -class network
  sudo ip addr show 
  sudo ip route show
  sudo tracepath forum.ubuntu.org.cn
  sudo apt-get install traceroute　
  sudo traceroute forum.ubuntu.org.cn
  ```

  


- 安装Google Pinyin

  https://www.jianshu.com/p/180cd9634b4a

  

- 软件安装到一半重装

  ```shell
  sudo apt-get install --reinstall name
  ```

- [Lantern](https://github.com/getlantern/lantern)

- [Typora](https://www.typora.io/#linux)

    ```shell
    # or run:

    # sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA300B7755AFCFAE
    wget -qO - https://typora.io/linux/public-key.asc | sudo apt-key add -

    # add Typora's repository

    sudo add-apt-repository 'deb https://typora.io/linux ./'

    sudo apt-get update

    # install typora

    sudo apt-get install typora

    ```

- [Pandoc](https://github.com/jgm/pandoc/releases/tag/2.9.2): Pandoc is a Haskell library for converting from one markup format to another, and a command-line tool that uses this library.

- [mathpix snipping Tool](https://mathpix.com/)

  ```shell
sudo snap install mathpix-snipping-tool
  ```

- [R](https://cloud.r-project.org/)

  ```shell
  sudo apt-get update
  sudo apt-get install r-base
  sudo apt-get install r-base-dev
  ```

- update R packages:

  ```shell
  sudo apt-get update
  sudo apt-get upgrade
  ```


- [RStudio](https://rstudio.com/products/rstudio/download/#download)

- [Anaconda 3](https://www.anaconda.com/products/individual) download [64-Bit (x86) Installer (522 MB)](https://repo.anaconda.com/archive/Anaconda3-2020.02-Linux-x86_64.sh)

```
cd Downloads
bash Anaconda3-`Press Tab`
```

​		[Python,Anaconda简介安装使用教程](https://www.jianshu.com/p/9a0172ae005f)

```
创建新环境
如果要安装指定的版本号，则只需要在包名后面以=和版本号的形式执行。如：conda create --name python2 python=2.7，即创建一个名为“python2”的环境，环境中安装版本为2.7的python。

如果要在新创建的环境中创建多个包，则直接在后以空格隔开，添加多个包名即可。如：conda create -n python3 python=3.5 numpy pandas，即创建一个名为“python3”的环境，环境中安装版本为3.5的python，同时也安装了numpy和pandas。
--name同样可以替换为-n。

显示已创建环境

conda info --envs
或
conda info -e
或
conda envlist

复制环境
conda create --name--clone
conda create --name py2 --clone python2，即为克隆名为“python2”的环境，克隆后的新环境名为“py2”。此时，环境中将同时存在“python2”和“py2”环境，且两个环境的配置相同。

删除环境
conda remove --name--all


```







- [QGIS](https://qgis.org/en/site/forusers/alldownloads.html#debian-ubuntu)
- [VS Code](https://code.visualstudio.com/Download#)
- [向日葵](https://sunlogin.oray.com/download/)
- 卸载向日葵

```
sudo dpkg -l | grep sunlogin
sudo dpkg -r sunloginclient
```

- [MySQL](https://www.cnblogs.com/opsprobe/p/9126864.html)

