---
title: 泛化调用
keywords: filter, 泛化调用
description: 泛化调用文档及说明
---

# 泛化调用

泛化接口调用方式主要用于客户端没有API接口及模型类元的情况，参数及返回值中的所有POJO均用map或者通用的数据结构（如json字符串等）表示，通常用于框架集成，比如：实现一个通用的服务测试框架，可通过`GenericService`调用所有服务实现。

目前，Dubbo-go已经实现了两种泛化调用的方式：map和protobuf-json，可以访问[apache/dubbo-go-samples](https://github.com/apache/dubbo-go-samples/tree/master/generic)查看使用实例，其中default是使用map方式，protobufjson是使用protobuf-json方式。

## 什么是泛化调用

## 序列化方式

### Map方式

支持的基础类型：

- int类型：int, int32, int64等
- uint类型：uint, uint32, uint64等

### Protobuf Json方式
