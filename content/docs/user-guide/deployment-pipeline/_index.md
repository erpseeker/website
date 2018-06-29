﻿+++
title = "应用和部署流水线"
description = "应用和部署流水线主要描述部署的环境、网络、域名、容器等，来告知用户如何部署和部署情况"
weight = 4
icon = "icon-deployment-pipeline"
+++

<h2 id="1">介绍</h2>

应用和部署流水线主要描述部署的环境、网络、域名、容器等，来告知用户如何部署和部署情况。

<h2 id="2">功能</h2>

 - [**环境流水线**](../deployment-pipeline/environment-pipeline) 是面向平台管理员、项目创建者和项目所有者根据不同用途配置相对应的环境信息。可以创建环境，删除环境，及对环境详情信息进行编辑修改。

 - [**应用市场**](../deployment-pipeline/application-market) 集合所有发布到本项目的应用，供用户浏览，可部署所需的应用及应用版本至项目中。

 - [**应用部署**](../deployment-pipeline/application-deployment) 提供可视化、一键式部署应用，支持并行部署和流水线无缝集成，实现部署环境标准化和部署过程自动化。
 
 - [**实例管理**](../deployment-pipeline/instance) 查看并且管理实例，进行实例的修改配置，启用停用等操作。

 - [**网络管理**](../deployment-pipeline/service) 是指内部的负载均衡以及网络转发，会将网络流量定向转发到指定的单个或者多个实例容器组，您可以通过选择需要负载和代理的实例，系统会为这些实例生成对应的负载规则。

 - [**域名管理**](../deployment-pipeline/ingress) 可以将您已经预定义好的域名规则在平台中进行配置，使外部能够通过指定的域名访问到系统内部的实例和网络。

 - [**容器管理**](../deployment-pipeline/container) 便于您查看和管理系统中的容器化实例，可以实时查看相关 pod 的状态以确定应用是否正常运行，同时可以查看对应的 pod日志进行错误定位和状态监控。