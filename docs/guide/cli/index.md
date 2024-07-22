---
nav:
  title: 指南
  order: -1
group:
  title: CLI 工具
  order: -1
---

# 使用
## 环境准备
首先需要安装 node, 并确保 node 版本在 14 以上。（推荐用 nvm 来管理 node 版本）
mac 或 linux 下安装 nvm。
```bash
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
$ nvm -v
0.39.1
```
安装 node。
```bash
$ nvm install 16
$ nvm use 16
$ node -v
v16.10.0
```

## 使用
```bash
da-cli -i /xxxx/company/node-h5 -t feature/dev-organ-miniprogram -b master
```
* -i 项目的目录地址
* -t 需要比较的目标分支，也可以是 commit hash
* -b 需要比较的基准分支, 也可以是 commit hash

## 结果
执行完上面的命令后会在项目目录产生一个`_analysisResult` 文件夹, 里面包含了生成的报告 html 和 res.json。其中 `res.json` 是执行结果：
```json
{
  // code 0 代表执行成功
  "code": 0,
  // resultUrl 是 CDN 地址
  "resultUrl": "xxxx"
}

```