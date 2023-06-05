# 云原生
 - https://u.geekbang.org/subject/cloudnative/1000797

## Go 语言特性
教学目标
1.理解 Go 语言基本语法
2.理解 Go 语言常用数据类型
3.理解 Go 语言常用小技巧
4.深入理解 Go 语言的多线程编程

针对的用户痛点
1.云原生从业者因为未熟练掌握 Go 语言，在阅读 Docker、containerd、Kubernetes 代码时有困难
2.未熟练掌握 Go 语言，在需要编写云原生组件时无法高效率高质量交付

通过学习掌握的核心能力
1.阅读 Go 语言代码的能力
2.用 Go 语言编写应用程序的基本能力
3.用 Go 语言编写一个 Kubernetes 中最常见的生产者消费者小程序

详细内容
1.Go 语言编译环境设置
2.Go 语言常用数据结构
3.Go 语言函数调用，深入理解 Channel 并基于 Channel 编写一个生产者消费者程序


## 使用 Go 语言编写一个小 Demo
教学目标
1.理解 Go 语言的调度原理
2.理解 Go 语言的内存管理
3.Go 语言依赖管理
4.Go 语言调试和问题分析 pprof

针对的用户痛点
1.对 Goroutine 无深入理解，无法利用 Go 语言强大的并发能力
2.面对众多的 Go 语言项目包依赖管理工具无所适从，不知道该用哪一个工具
3.针对 Go 语言编写的程序，不知道如何调试

通过学习掌握的核心能力
1.了解 Go 语言的高级话题，如线程调度原理，内存管理等，使得学员有能力编写高效程序
2.理解 Go 语言的依赖管理方法，以便能够正确地管理项目依赖
3.学会用 pprof 对应用运行时的调用栈、内存等进行分析
4.学会用 Go 语言编写一个简单的 HTTP 服务器供后续云原生应用使用

详细内容
1.Goroutine 的调度
2.内存管理
3.学会用 Go 语言编写一个简单的 HTTP 服务器


## Docker 核心技术
教学目标
1.理解容器特性以及相比虚拟化技术所具备的优势
2.了解容器技术的实现细节：namespace、cgroup、文件系统

针对的用户痛点
1.分不清容器技术和虚拟化技术的差异，在做技术决策时没有理论支撑
2.因为不了解技术原理，排查容器问题时毫无头绪

通过学习掌握的核心能力
1.了解 namespace 技术的原理以及基于 namespace 的问题排查方法
2.理解 cgroup 控制资源限额的方法，查看 cgroup 配置并临时调整 cgroup 配置
3.理解容器文件系统如何高效管理运行时和数据
4.理解容器网络，为进一步理解 Kubernetes 网络插件奠定基础
5.基于 Dockerfile 将应用程序打包成容器镜像

详细内容
1.容器技术的本质以及技术优势，namespace、cgroup、文件系统、网络连通
2.容器镜像与镜像仓库
3.将 Go 语言编写的 HTTP 服务器打包成容器镜像


## Kubernetes 架构原则和对象设计
教学目标
1.理解 Kubenretes 架构原则
2.理解 Kubernetes 的对象设计与 API 定义
3.理解 Kubernetes 控制器模式与多组件联动机制

针对的用户痛点
1.对 Kubernetes 有简单认知，但无法编写出高效的、符合云原生规范和最佳实践的组件
2.对组件和基本对象只有浅层次的理解，对 API 的统一性和差异性无深入理解
3.不了解 Kubernetes 的控制器原理，对 Kubernetes 控制面板组件如何运作无深入理解

通过学习掌握的核心能力
1.动手搭建 Kubernetes 环境
2.理解 Kubernetes 架构原则
3.理解 Kubernetes API 定义的设计原则，理解 Kubernetes 对象中的重要属性
4.理解 Kubernetes 控制器的联动机制

详细内容
1.环境搭建
2.Kubernetes 架构优势及架构原则
3.Kubernetes 核心组件
4.Kubernetes 对象设计与 API 定义
5.Kubernetes 控制器模式


## Kubernetes 控制平面组件：etcd
教学目标
1.深入理解 Kubernetes 的唯一数据存储组件 etcd
2.掌握构建生产系统中 etcd 集群的方法
3.熟悉 etcd 的优化管理，了解灾备方案

针对的用户痛点
1.对 etcd 的实现机制不了解，不知道在生产化应用过程中可能遇到的问题
2.不知道应该如何构建生产系统中的 etcd 集群
3.不知道如何进行数据的备份和灾难恢复

通过学习掌握的核心能力
1.理解 Raft 协议的工作机制和 etcd 的实现原理，针对 etcd 生产系统的配置优化以及数据灾备
2.深入理解 API Server 的实现机制，包括与企业认证系统整合、鉴权、准入插件的实现等等
3.深入理解 Kubernetes 的对象实现
4.如何构建高可用的 etcd 和 API Server 控制平面

详细内容
1.深入理解 Kubernetes 的数据存储 etcd
2.了解 Raft 协议
3.生产系统中 etcd 的配置
4.etcd operator
5.etcd 的灾备方案生产系统中常见问题解析


## Kubernetes 控制平面组件：API Server
教学目标
1.深入理解 Kubernetes API Server 的实现机制
2.掌握基于 API Server Webhook 的整合方案

针对的用户痛点
1.缺乏对 Kubernetes 对象实现方法的理解
2.对 API Server 缺乏理解，不知道如何与企业认证系统整合，不会基于鉴权准入等机制打造多租户 Kubernetes 平台

通过学习掌握的核心能力
1.理解 Kubernetes 对象设计的实现机制
2.理解 API Server 缓存的工作机制
3.掌握生产系统中 API Server 的常用配置
4.掌握 API Server 与企业生态系统的整合方法

详细内容
1. 深入理解 Kubernetes API Server
    1.1 API Server 代码走读
    1.2 理解 internalVersion、externalVersion 和 storageVersion
    1.3 理解 conversion
    1.4 基于 client-go 生成 Kubernetes 框架代码
    1.5 理解 lister 和 informer 框架

2. 理解 API Server 缓存
3. API Server 与企业生态系统的整合：认证接入、鉴权、准入控制
4. API Server 常用配置与常见问题解析


## Kubernetes 控制平面组件：调度器和控制器
教学目标
1.理解 Kubernetes 调度器原理以及常用调度插件
2.理解 Kubernetes 调度的常用技巧，利用亲和性与反亲和性进行调度
3.理解 Kubernetes 的常见控制器
4.深入理解 Kubelet 对 Pod 声明周期的管理

针对的用户痛点
1.对 Kubernetes 调度器无深入理解，在 Pod 无法调度时，不知道如何排查问题
2.不会利用 Kubernetes 调度器实现应用的高效、高可用部署
3.对 Kubernetes 控制器缺乏全面认知
4.对 Kubernetes 如何管理 Pod 生命周期缺乏认知

通过学习掌握的核心能力
1.排查调度故障，利用调度器实现应用的高可用部署
2.扩展对 Kubernetes 控制器的认知，理解更多的 Kubernetes 控制平面行为
3.深入理解 CRI、CNI 和 CSI

详细内容
1. 深入理解 Kubernetes 调度器
2. 深入理解 Kubenretes 控制器
3. 深入理解 Kubelet
    3.1 如何运行你的 Pod（CRI、CNI、CSI）
    3.2 Kubelet Pod 代码走读
    3.3 containerd 代码走读
    3.4 CNI 代码走读
    3.5 全方位的 CSI 一站式解决方案：Rook


## Kubernetes 控制平面组件：生命周期管理和服务发现
教学目标
1.深入理解 Pod 的完整生命周期和就绪状态控制
2.深入理解 Pod 状态控制对应用可用性的影响
3.深入理解 Kubernetes 中的服务发现机制，包括负载均衡配置和域名服务

针对的用户痛点
1.解决日常运维的困扰，比如，在 Pod 初始化或故障转移时或者版本发布时，如何不影响业务？
2.我发布的服务经常出现服务中断，是缺了什么配置吗？

通过学习掌握的核心能力
1.理解 Pod 的完整生命周期，如何初始化、如何控制就绪状态、如何探活、如何优雅终止
2.如何发布服务，如何剔出异常实例

详细内容
1.深入理解 Kubernetes 的服务实例对象 Pod：Pod 生命周期详解、健康探针、ReadinessGate
2.深入理解 Kube-Proxy：如何发布你的服务、代码走读、负载均衡配置
3.域名管理
4.基于 Ingress 以及 Service API 的入站流量管理



## 生产化集群的管理
教学目标
1.掌握生产化集群的搭建技术
2.掌握生产化集群持续运维过程中最重要的节点管理能力
3.如何在不影响业务的前提下完成 Kubernetes 升级

针对的用户痛点
1.不知道如何快速构建本地集群供研发测试使用
2.未掌握构建生产化集群的方法，缺少对集群节点的管控，节点出现故障以后需要人为介入
3.如何实现生产化集群的管理，比如计算节点的监控与管理
4.不了解完成了集群搭建以后离生产化还有多远

通过学习掌握的核心能力
1.快速构建本地集群的能力
2.理解 Kubernetes 集群构建的原理，掌握搭建 Kubernetes 集群的能力
3.基于 Cluster API 完成生产化集群的构建和持续运维

详细内容
1.利用 kind 构建本地集群
2.利用 kubeadm 构建基于虚拟机的集群
3.利用 Cluster API 完成生产化集群的搭建
4.持续运维的考量：节点健康检查、Kubernetes 升级、主机操作系统升级


## Kubernetes 的生产化运维
教学目标
1.如何实现基于 Kubernetes 的 CI/CD
2.如何实现生产化集群的监控

针对的用户痛点
1.缺少企业统一的镜像仓库
2.镜像安全应该如何保证
3.企业缺少持续集成持续部署能力
4.缺少对整个集群的监控，希望实现无人值守

通过学习掌握的核心能力
1.打造持续集成平台
2.基于自动化管理生产化集群实现对集群
3.控制面板以及重要应用的监控和告警

详细内容
1.镜像仓库和容器镜像缓存
2.镜像扫描和镜像安全保证
3.基于 Kubernetes、Jekins、Tekton 打造 CI/CD Pipeline
4.集群监控：日志收集和分析，事件、指标和告警（Event、Metrics 和 Alert）



## 将应用迁移至 Kubernetes 平台
教学目标
1.如何将无状态应用发布到 Kubernetes 平台
2.如何基于 Kubernetes 原生能力将有状态应用发布到 Kubernetes 平台
3.基于 Kubernetes 对象扩展，将更复杂的应用发布到 Kubernetes 平台

针对的用户痛点
1.缺少将应用发布到 Kubernetes 平台上的理论指导
2.对于有状态应用，更不知道如何借助 Kubernetes 平台的优势进行处理

通过学习掌握的核心能力
1.掌握 Kubernetes 提供的应用管理框架，包括有状态应用和无状态应用
2.掌握 Operator 模式，具备通过 Kubebuilder 构建自己的 CRD，并且基于 CRD 编写控制器的能力
3.利用 Kubebuilder 完成控制器的测试和发布
4.借助 Helm 完成复杂的应用模板管理

详细内容
1.应用容器化
2.无状态应用移植到 Kubernetes 平台的考量
3.有状态应用移植到 Kubernetes 平台的考量
4.理解 Operator
5.借助 Kubebuilder 开发一个 Operator
6.借助 Helm 管理应用发布


## 基于 Istio 的高级流量管理
教学目标
1.理解基于 TCP/UDP 协议的 Kubernetes Service 的局限性
2.理解 Kubernetes 入站流量管理的场景和原生方案
3.理解原生方案的局限性和社区的方向
4.深入理解 Envoy 的服务发现机制、线程模型以及扩展机制
5.理解如何基于 Istio 实现入站、出站流量管理以及服务网格管理

针对的用户痛点
1.社区的 Ingress 对象无法毕业，为支持生产化应用，应该用什么方案提供入站流量支撑
2.Envoy 为什么变成了 Kubernetes 中七层代理的首选
3.社区爆火的 Istio 背后的技术驱动力是什么，我应该选 Istio 作为入站流量管理平面组件吗

通过学习掌握的核心能力
1.深入理解 Envoy 的实现机制
2.深入理解 Istio 的实现机制，了解为什么 Istio 会成为服务网格的标准

详细内容
1.入站流量管理 Ingress 和 Service API
2.Istio 和 Envoy
3.深入理解 Envoy：发现机制、线程模型、filter 机制、高级特性
4.深入理解 Isito：入站流量、出站流量、Service Mesh（服务网格）、Istio 服务发现代码走读
5.安全保证


## Kubernetes 集群联邦和 Istio 多集群管理
教学目标
1.如何通过集群联邦的统一控制平面管理多个集群
2.如何部署跨地域的高可用应用
3.如何通过 Istio 多集群方案管理跨集群的 Service Mesh（服务网格）

针对的用户痛点
1.针对真正的生产化应用，跨地域部署是确保应用高可用的一个强需求，那么如何管理多个 Kubernetes 集群
2.针对跨集群部署的应用，如何确保其接入流量高可用，如何借助 Istio 实现这一目的

通过学习掌握的核心能力
1.Kubernetes 集群联邦的实现原理和配置方法
2.Istio 多集群实现原理和配置方法

详细内容
1.Kubernetes 集群联邦
2.基于集群联邦的跨地域高可用部署
3.基于 Istio 多集群的流量高可用方案


基于 Kubernetes 和 Istio 的安全保证
教学目标
1.理解传统安全架构的挑战
2.掌握零信任架构的意义和机遇
3.掌握 Kubernetes 平台本身的安全保证手段
4.学习如何基于 Kubernetes 和 Istio 实现对应用的隔离和安全保证

针对的用户痛点
1.如何确保 Kubernetes 平台的安全性
2.如何确保 Kubernetes 中数据保存的安全性
3.如何确保 Kubernetes 上运行应用的安全性

通过学习掌握的核心能力
1.如何保证 etcd 中保存的数据安全性
2.如何保证 Kubernetes 控制面板的安全性
3.如何确保 API 网关的安全性
4.对应用进行安全隔离
5.如何基于零信任架构完成应用的认证和授权

详细内容
1.理解 etcd 的加密方法
2.掌握 Kubernetes 控制面板的安全配置
3.掌握应用隔离的常规手段以及在 Kubernetes 中配置的方式
4.掌握 API 网关的安全配置
5.了解基于 Istio 的认证鉴权机制


## 微服务项目的开发和部署案例
教学目标
完成一个复杂的异构的微服务系统在 Kubernetes 平台上的部署，以 Istio 的 Bookinfo 为例

针对的用户痛点
1.随着业务复杂度的增加，微服务的部署和运维变得越来越有挑战性，如何保证微服务应用部署的高性能是一个复杂问题
2.如何基于熔断、限流等手段保护核心业务
3.如何基于基础架构平台确保应用安全

通过学习掌握的核心能力
1.基于微服务架构的复杂应用部署
2.熔断、限流、故障注入
3.应用的安全保证

详细内容
本模块是之前所有模块的综合复习模块，希望借助本模块完成基于 Kubernetes 框架下面微服务治理这一重要命题的回顾和总结。