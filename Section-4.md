# Section 4

## 学习目标

修改已提交文件

版本回退

撤回工作区修改

## 修改文件

1. 直接修改`readme.md`文件

   ```shell
   vim readme.md
   
   #进行一定修改
   ```

2. 查看文件是否修改

   ```shell
   git status
   ```

3. 查看具体修改内容 

   ```shell
   git diff readme.md
   ```

4. 提交修改后版本

   ```
   git commit -m "修改第一次<修改说明>"
   ```

## 版本回退

1. 查看日志，作出过哪些修改

   ```shell
   git log
   git log --oneline #查看历史记录的简洁的版本
   git log --graph #查看历史分支、合并，拓扑图
   git log --reverse #逆向显示所有日志
   git log --author #指定用户
   
   #指定时间
   --since 
   --before
   --until
   --after
   ```

2. 回退

   ```shell
   #方案一
   #回退到前 100 个版本
   git reset --hard HEAD~100
   ```

   ```shell
   #方案二
   #回退到前 1 个版本
   git reset --hard HEAD^
   #回退到前 2 个版本
   git reset --hard HEAD^^
   ```

   ```shell
   #方案三
   #先查看版本号
   git reflog
   #参数写需要返回的版本的版本号 
   git reset --hard <版本号>
   ```

## 丢弃工作区修改

以下两种情况本质上是一样的

1. 情景：再修改了工作区文件还没有提交缓存区的时候，想返回之前版本

2. 例如 `readme.md`

   ```shell
   git checkout -- readme.md
   ```

1. 情景你删除了某一个工作区文件，还未发布到缓存区，想撤回删除操作（其实也是返回之前的版本）

2. 例如 `readme.md`

   ```shell
   git checkout -- readme.md
   ```


## 其他修改

| 命令             | 说明                                 | 备注 |
| ---------------- | ------------------------------------ | ---- |
| git rm           | 将文件从暂存区和工作区中删除         |      |
| git mv           | 移动或重命名工作区文件               |      |
| git blame <file> | 以列表形式查看指定文件的历史修改记录 |      |















