---
typora-copy-images-to: picture
---

# Section 7

## 学习目标

添加远程库

Github

Gitee

## 概念梳理

新概念：远程仓库

作用：将数据放在一台其他人员能链接的服务器上

- workspace：工作区
- staging area：暂存区/缓存区
- local repository：版本库或本地仓库
- remote repository：远程仓库

图解

![1663658965680](.\picture\1663658965680.png)

## Github 添加远程库

1. 生成 SSH Key

   ```shell
   ssh-keygen -t rsa -C "youremail@example.com"
   
   #youremail@example.com 你的GitHub邮箱
   ```

2. 查看密钥

   > 在 ~/ 下新生成的 .ssh 文件夹，打开 id_rsa.pub，复制里面的 key

3. 打开 [GitHub](https://github.com/)

   > 1.  Account => Settings（账户配置）
   > 2. SSH and GPG keys
   > 3. New SSH key
   > 4. title 设置标题 （这一对 ssh 的名字）
   > 5. Key 粘贴刚刚的复制

4. 连通

   ```shell
   ssh -T git@github.com
   ```

5. 再次进入 [GitHub](https://github.com/)
   常规流程新建仓库

6. 本地仓库提交远程仓库

   > 1. 添加远程版本库
   >
   > ```shell
   > git remote add [shortname] [url]
   > ```
   >
   > ```shell
   > git remote add origin https://github.com/xiao-ge4/git-learning
   > 
   > #"https://github.com/xiao-ge4/git-learning"是我的地址，修改为自己的地址
   > 
   > #origin 是远程仓库的名字，这是Git默认的叫法，也可以改成别的
   > ```
   >
   > 2. 本地库的所有内容推送到远程库上
   >
   > ```shell
   > git push -u origin master
   > 
   > #把本地仓库分支 master 的内容推送到 origin 去
   > ```
   >
   > 3. 注意
   >
   >    > 这里是2次用户名密码：第一次是 Github 的登陆用户名和密码，第二次是输入 token 生成的用户名和密码（具体生成步骤如下）
   >    >
   >    > 1. 进入[GitHub](https://github.com/) 进入 Settings
   >    > 2. 左侧 Developer settings
   >    > 3. 左侧 Personal access tokens
   >    > 4. 右上 Generate new token
   >    > 5. 填写 用户名，勾选 权限
   >    > 6. 生成账号，复制密码

## 相关指令

git remote

| 命令                                | 作用                   | 备注 |
| ----------------------------------- | ---------------------- | ---- |
| git remote                          | 查看当前远程仓库       |      |
| git remote -v                       | 显示所有远程仓库       |      |
| git remote show [remote]            | 显示某个远程仓库的信息 |      |
| git remote add [shortname] [url]    | 添加远程版本库         |      |
| git remote rm name                  | 删除远程仓库           |      |
| git remote rename old_name new_name | 修改仓库名             |      |

| 命令                 | 作用                                   | 备注                                                    |
| -------------------- | -------------------------------------- | ------------------------------------------------------- |
| git fetch            | 从远程库下载新分支与数据               | 该命令执行完后需要执行 git merge 远程分支到你所在的分支 |
| git merge            | 从远端仓库提取数据并尝试合并到当前分支 |                                                         |
| git pull             | 下载远程代码并合并                     |                                                         |
| git push             | 上传远程代码并合并                     |                                                         |
| git remote rm [别名] | 删除远程仓库                           |                                                         |

## Gitee 添加远程库



## 私有服务器


















