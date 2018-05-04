+++
title = "实例管理"
weight = 6
+++

# 实例管理

实例管理界面只显示平台已有实例，用户只能进行查询实例、查看实例详情和更改实例配置的操作。

实例与微服务的关系：微服务与实例为一对多的从属关系。一个微服务可以有多个实例，一个实例只能属于一个微服务。

实例与配置的关系：配置与实例为一对多的应用关系。同一个微服务下，一个配置可以被多个实例应用，一个实例只能应用一个配置。

**功能：**

- [实例列表](#1)
- [实例查询](#2)
- [实例详情](#3)
- [应用配置](#4)


<h2 id="1">实例列表</h2>

列表字段：

- **实例ID**：实例ID具有唯一性，是实例的标识。实例ID的展示形式为`<主机名>:<所属微服务>:<端口号>`。
- 实例状态：一般为UP、DOWN特定字段值。
- 所属微服务：为微服务名称，因为微服务名称是微服务的标识。一个实例只能属于一个微服务，一个微服务可以有多个实例。

<h2 id="2">实例查询</h2>

**必填项：**

可查询字段：

- **实例ID**：选中实例ID字段，搜索框下方出现所有实例ID的列表。可以继续输入目标实例ID进行过滤，下方实例ID列表随输入值实时更新，输入值最好为`<主机名>:<所属微服务>:<端口号>`形式。最后可以选中实例ID列表的列表项，或输入正确的实例ID按回车键进行提交。
- 实例状态：选中实例状态字段，搜索框下方出现所有实例状态的列表，一般为UP、DOWN两个列表项。
- 所属微服务：选中所属微服务字段，搜索框下方出现所有实例所属微服务的列表。选中一个微服务名称，则实例列表列出所有属于该微服务的实例。
    

<h2 id="3">实例详情</h2>

详情字段：

- **实例ID**：实例ID的展示形式为`<主机名>:<所属微服务>:<端口号>`。实例ID具有唯一性，是实例的标识。
- 主机名：分配给实例的地址。
- IP：实例的实际地址。
- 所属微服务：实例属于的微服务的微服务名称。
- 端口号：实例的端口号。
- 上次注册时间：实例上一层注册的时间。
- 元数据：可以有多条数据项。每条数据项为名字-值的组合。

<h2 id="3">应用配置</h2>

即实例应用配置。一个实例只能应用一个配置。

配置列表字段为配置ID，因为配置ID是配置的标识。列表为实例所属服务下的所有配置。

下图为同一个微服务下，实例应用配置的关系图。

![实例应用配置关系图](/docs/user-guide/api/image/instance_config.png)