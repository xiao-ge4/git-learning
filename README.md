# git-learning
A series of documents for learning git

## 概述

- 开源
- 分布式
- 版本控制系统
- Linus Torvalds 为了帮助管理 Linux 内核开发而开发的一个开放源码的版本控制软件

### 说明

- 分布式 vs 集中式

  > 1. 集中式
  >    - 定义：版本库是集中存放在中央服务器的，而干活的时候，用的都是自己的电脑，所以要先从中央服务器取得最新的版本，然后开始干活，干完活了，再把自己的活推送给中央服务器
  >    - 缺点：必须联网
  > 2. 分布式
  >    - 定义：没有“中央服务器”，每个人的电脑上都是一个完整的版本库（就不需要联网了），通信只用推送修改内容（不用推送整个版本库）
  >    - 优点：安全性高（独立的完整库，不受中央控制器状态影响）、不需要联网

## 参考来源/推荐资料

- [集中式vs分布式 - 廖雪峰的官方网站 (liaoxuefeng.com)](https://www.liaoxuefeng.com/wiki/896043488029600/896202780297248)

  > 语言通俗，但文字太多，符合 0基础

- [Git 安装配置 | 菜鸟教程 (runoob.com)](https://www.runoob.com/git/git-install-setup.html)

  > 简洁但较完整，符合一点基础

- [github-git-cheat-sheet (runoob.com)](https://www.runoob.com/manual/github-git-cheat-sheet.pdf)

  > Git 完整命令手册 PDFv

- [Git - Reference (git-scm.com)](https://git-scm.com/docs)

  > Git 完整命令手册 网页版

- [git 简明指南 (runoob.com)](https://www.runoob.com/manual/git-guide/)

  > 简明教程（非常简洁）

- 我的这个！

  > 1. 有 md 版，可下载后自己修改
  > 2. 易查找知识点（手册）
  > 3. 也有解释性语句

## 学习目录

老规矩，后面章节学习梗概



| 章节 | 目标                                               | 备注                              |
| ---- | -------------------------------------------------- | --------------------------------- |
| 1    | 环境部署                                           | Linux Windows Mac                 |
| 2    | 工作流程 及 相关概念                               | 工作区 暂存区 版本库              |
| 3    | 创建仓库<br />拷贝仓库<br />文件提交到仓库         |                                   |
| 4    | 修改已提交的文件<br />版本回退<br />撤回工作区修改 |                                   |
| 5    | 分支管理                                           |                                   |
| 6    | 标签<br />记录重要节点                             |                                   |
| 7    | 添加远程仓库                                       | Github<br />Gitee<br />私有服务器 |
| Q&A  |                                                    | 过程中的问题解决                  |

