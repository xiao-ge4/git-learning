---
typora-copy-images-to: picture
---

# Section 3

## 学习目标

创建 版本库/仓库/repository

拷贝 仓库

文件添加到仓库

## 创建仓库

1. 创建文件夹

	```shell
	mkdir testGit
	```
	
	以上命令是在 Git Bash 中执行，默认位置`c/user/<username>`比如我的位置
	![1663555170041](.\picture\1663555170041.png)
	
2. 进入文件夹，打印位置检查

   ```shell
   cd testGit #进入
   pwd #显示当前位置
   ```

   ![1663555307986](.\picture\1663555307986.png)

3. 初始化 仓库

   ```shell
   git init
   ```

4. 检查初始化

   ```
   ls #列出所有文件
   ls -al #列出包括隐藏文件，上次改动时间、权限等参数信息
   ```

   ![1663555522034](.\picture\1663555522034.png)

## 拷贝仓库

上命令

```shell
git clone <repo>
git clone <repo> <directory>

#repo 仓库（在github gitee上拷贝，如下图）
#directory 本地目录
```

![1663555830305](.\picture\1663555830305.png)

## 添文件到仓库

1. 在仓库目录下新建`readme.md`作为说明文件

2. 写入内容

3. 将文件从工作区添加到缓存区

   ```shell
   git add readme.md 
   ```
   
4. 文件从缓存库提交到仓库

   ```shell
   git commit -m "说明文字"
   ```

5. 查看是否还有文件未提交

   ```shell
   git status
   ```



   

​    

   







