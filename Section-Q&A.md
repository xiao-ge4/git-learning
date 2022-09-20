# Section Q&A

## 学习目标

各种问题的记录





### 本地库推送到远程库

```shell
git push -u origin master

#把本地仓库分支 master 的内容推送到 origin 去
```

> 这里是2次用户名密码：第一次是 Github 的登陆用户名和密码，第二次是输入 token 生成的用户名和密码（具体生成步骤如下）
>
> 1. 进入[GitHub](https://github.com/) 进入 Settings
> 2. 左侧 Developer settings
> 3. 左侧 Personal access tokens
> 4. 右上 Generate new token
> 5. 填写 用户名，勾选 权限
> 6. 生成账号，复制密码

### Git HEAD detached from origin

解释：意思是现在 Git HEAD 处于游离状态

1. 查看现在的 commit 号、记录

   ```shell
   git branch -v
   ```

2. 到另一个分支下，将他合并过来（如果目前仓库里的东西还需要的话）

   ```shell
   git merge <commit号>
   ```

   















