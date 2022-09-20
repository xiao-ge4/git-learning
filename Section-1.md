# Section 1

## 目标

环境部署 ：Linux Windows Mac

## Linux

Debian / Ubuntu （没有 Centos/RedHat ）

安装依赖

> ```shell
> apt-get install libcurl4-gnutls-dev libexpat1-dev gettext libz-dev libssl-dev
> ```

安装 git

> 1. apt 安装
>
> 	```shell
> 	apt-get install git
> 	```
>
> 2. 源码安装
>
>    1. 在[Git - Downloads (git-scm.com)](https://git-scm.com/download)下载最新源码包
>
>    2. 解压安装下载的源码包
>
>       ```shell
>       tar -zxf <你的下载包名称>
>       cd <解压后的包的名称>
>       make prefix=/usr/local all #编译
>       sudo make prefix=/usr/local install #安装
>       ```
>
>       
>
> 3. 检验安装是否成功
>
>    ```shell
>     git --version
>    ```
>

## Windows

这里有一步一步的教程

> [Windows系统Git安装教程（详解Git安装过程） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/242540359)

下载 exe 文件

> 1. 官网地址[Git for Windows](https://gitforwindows.org/)
> 2. 国内镜像[CNPM Binaries Mirror (npmmirror.com)](https://registry.npmmirror.com/binary.html?path=git-for-windows/)

点击运行安装

在 Git Bash 可以直接输入 git 命令了

## Mac

图形化工具

> [git-osx-installer download | SourceForge.net](https://sourceforge.net/projects/git-osx-installer/)

## Git 配置

Git 提供了一个叫做 git config 的工具，专门用来配置或读取相应的工作环境变量。

变量位置

> 这些变量可以存放在以下三个不同的地方：
>
> 1. `/etc/gitconfig` 文件：系统中对所有用户都普遍适用的配置。若使用 `git config` 时用 `--system` 选项，读写的就是这个文件
> 2. `~/.gitconfig` 文件：用户目录下的配置文件只适用于该用户。若使用 `git config` 时用 `--global` 选项，读写的就是这个文件
> 3. `.git/config` 文件：这里的配置仅仅针对当前项目有效。每一个级别的配置都会覆盖上层的相同配置，所以 `.git/config` 里的配置会覆盖 `/etc/gitconfig` 中的同名变量
>
> 在 Windows 系统上，Git 会找寻用户主目录下的 .gitconfig 文件。主目录即 $HOME 变量指定的目录，一般都是 C:\Documents and Settings\$USER

用户信息

> ```shell
> git config --global user.name "runoob"
> git config --global user.email test@runoob.com
> ```
>
> 如果用了 --global 选项，那么更改的配置文件就是位于你用户主目录下的那个，以后你所有的项目都会默认使用这里配置的用户信息
>
> 如果要在某个特定的项目中使用其他名字或者电邮，重新配置即可

文本编辑器

> 一般可能会是 Vi 或者 Vim
>
> 也可以设置
>
> ```shell
> git config --global core.editor emacs
> ```

查看配置信息

> ```shell
> git config --list
> http.postbuffer=2M
> user.name=runoob
> user.email=test@runoob.com
> ```