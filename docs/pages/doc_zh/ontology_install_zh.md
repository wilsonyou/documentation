---
title: 
sidebar: ont_doc_zh
permalink: ontology_install_zh.html
folder: doc_zh
---

[English](./ontology_install_en.html) / 中文

<h1 align="center">安装 </h1>
<p align="center" class="version">版本 1.0.0 </p>

## 构建开发环境
成功编译ontology需要以下准备：

* Golang版本在1.9及以上
* 安装第三方包管理工具glide
* 正确的Go语言开发环境
* Golang所支持的操作系统

## 部署|获取ontology
### 从源码获取
克隆ontology仓库到 **$GOPATH/src/github.com/ontio** 目录

```shell
$ git clone https://github.com/ontio/ontology.git
```
或者
```shell
$ go get github.com/ontio/ontology
```

用第三方包管理工具glide拉取依赖库

````shell
$ cd $GOPATH/src/github.com/ontio/ontology
$ glide install
````

用make编译源码

```shell
$ make
```

成功编译后会生成两个可以执行程序

* `ontology`: 节点程序/以命令行方式提供的节点控制程序
* `tools/sigsvr`: (可选)签名服务 - sigsvr是一个签名服务的server以满足一些特殊的需求。详细的文档可以在[这里](./sigsvr_zh.html)参考

### 从release获取
You can download at [release page](https://github.com/ontio/ontology/releases).