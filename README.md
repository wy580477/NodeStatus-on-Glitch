# NodeStatus-on-Glitch

## 鸣谢

- [cokemine/nodestatus](https://github.com/cokemine/nodestatus)

## 概述

本项目用于在 Glitch 免费服务上部署 NodeStatus 探针服务端。

## 注意

 **请勿滥用，账号封禁风险自负。**
 
## 变量

对部署时设定的变量做如下说明。

| 变量 | 默认值 | 说明 |
| :--- | :--- | :--- |
| `DATABASE` | `` | 数据库连接 URL |
| `WEB_PASSWORD` | `` | 管理面板密码 |
| `NO_HEADER` | `Enable` | 禁用标题图片 |
| `WEB_TITLE` | `` | 标题文字 |
| `WEB_SUBTITLE` | `` | 副标题文字 |

更多变量设置详见： https://github.com/cokemine/nodestatus#environment

## 数据持久化

由于免费 Glitch 项目只能是公开项目，强烈建议连接外部数据库。

**bit.to 将于 2023.6.29 停止服务**

elephantsql 免费 PostgreSQL 数据库

1. 前往 https://www.elephantsql.com 注册账号，并新建一个数据库。
2. 点击数据库名称，进入数据库管理页面，右侧的 Details 下方，复制 "URL" 项即为数据库连接 URL。


## 部署

前往 glitch.com 注册账户，然后点击下面按钮：

[![Remix on Glitch](https://cdn.glitch.com/2703baf2-b643-4da7-ab91-7ee2a2d00b5b%2Fremix-button.svg)](https://glitch.com/edit/#!/import/github/wy580477/NodeStatus-on-Glitch)

点击左侧文件列表中的 .env 文件，按上文所述设置环境变量。

然后点击页面下方 TERMINAL，执行 refresh 命令，稍等片刻即部署完成。

## 通过 Cloudflare 反向代理设置自定义域名

https://github.com/wy580477/PaaS-Related/blob/main/CF_Workers_Reverse_Proxy_chs_simple.md
