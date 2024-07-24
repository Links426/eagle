---
nav:
  title: 指南
  order: -1
group:
  title: 介绍
  order: 2
---

# 快速上手
本项目大致使用流程如下：
1. 准备一个种子项目
2. 前端开发同学使用脚手架，创建新项目
3. 种子项目更新
4. 前端开发同学拉取种子的更新，在本地进行更新项选择
5. push，完成更新

## 安装脚手架

全局安装 eagle-cli
```shell

npm install -g @tencent/eagle-cli

```

## cli 使用

* add <registry-name> <registry-url>  新增种子项目
* create <registry-name> 创建一个新的项目
* delete <registry-name> 删除指定名字的种子项目
* ls 展示所有的种子项目
* publishLocal 将本地的种子项目链接更新发布同步  
* updateLocal 检查当前项目更新  
* update 同步拉取种子项目的更新

## 结果
```shell

eagle update

```

如果本地已经添加了种子项目的远端链接，执行完上面的命令后，VSC的源代码管理 ```control + shift + G``` 会自动提示更新了哪些，在这里选择想要的更新，直接点击提交，并push本地代码到对应的分支即可～