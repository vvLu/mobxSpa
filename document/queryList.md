# 中后台项目 - 查询表格业务最佳实践

## 前言

查询表格业务是中后台系统最常用的业务系统之一，我相信该业务场景会在你的项目中会大量出现。既然该此场景在项目中大量的出现，所以对其进行必要的封装会极大的提升业务的复用性以及项目的可维护性。以下是不采取封装可能会带来的问题。

- 会出现大量重复的业务代码
- 不同开发人员对公共业务实现的 方式/命名 不同
- 在 store 层，不同的开发人员可能会定义不同的数据模型
- 相同业务的代码分散，不利于形成良好的开发规范

以上的几点总结起来就是不利于项目的维护和形成规范。

## 查询表格业务 - 设计思路

该业务场景如此常见，所有相信大家都有自己的实现。所以这里仅仅是提出一个设计思路，你可以用来参考案然后考虑是否对你的项目有帮助。设计图如下；