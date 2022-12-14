---
typora-copy-images-to: picture
---

# Section 2

## 学习目标

Git 工作流程

相关概念：工作区 暂存区 版本库

## 流程

- 克隆 Git 资源作为工作目录。
- 在克隆的资源上添加或修改文件。
- 如果其他人修改了，你可以更新资源。
- 在提交前查看修改。
- 提交修改。
- 在修改完成后，如果发现错误，可以撤回提交并再次修改并提交。

图解

> 注意箭头的指向

![1663552316955](.\picture\1663552316955.png)

## 工作空间

这里只是大概说明，代码示例会放在后面

### 工作区 

位置：电脑里能看到的目录

### 暂存区

英文：stage 或 index

位置：一般存放在 `.git` 目录下的 index 文件（.git/index）中

### 版本库

位置：工作区一个隐藏目录 `.git`，这个不算工作区，而是 Git 的版本库

### 图示

![20220919103107](.\picture\20220919103107.jpg)









