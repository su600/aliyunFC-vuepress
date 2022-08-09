# Su 技术体系

## 工业互联网技术

### 工业自动化

- 西门子

	- PLC

		- S7-200、300
		- S7-1200

			- v4.4固件支持OPC UA

		- S7-1500

	- 数控系统

		- 840D

	- TIA 博途
	- Industrial Edge

		- nano
		- 2040
		- 2050

- 倍福PLC、TwinCAT
- 罗克韦尔AB PLC
- 发那科

	- 机器人
	- 数控系统
	- Focas

- Kuka机器人
- UR协作机器人

	- NodeRed
	- ROS

- Straton Editor
- CoDeSys软PLC
- OpenPLC

### 工业通讯

- Profinet、ProfiNet
- EtherCAT
- EtherNET/IP
- OPC UA

	- UaExpert
	- 西门子UA信息模型编辑器
	- SDK

		- Python SDK
		- Prosys Java SDK
		- Markiton C++ SDK
		- 62541 pub/sub

- RFID
- 赫优讯
- TSN

	- OPC UA over TSN

- NC-Link
- MTConnect

### 数据采集

- 西门子S7

	- pysnap7

- OPC UA

	- async-ua

		- 证书加密登录未解决

			- Basic256Sha256

- 倍福ADS

	- pyads

		- 变量表扫描
		- ads路由添加（仅linux）

- 罗克韦尔CIP

	- pylogix

		- 设备扫描
		- 变量表扫描

- Modbus

	- 仪表、能耗

- Docker容器化
- 发那科Focas

	- Dll/so文件

- TCP/IP
- socket
- SCADA
- PTC Kepware
- Ignition等

### Python

- Flask

	- Flask-Bootstrap
	- Flash
	- BluePrint
	- Flask-RESTful
	- Flask 2.0
	- Docker容器

- 数据采集
- MQTT
- Pandas数据处理
- Streamlit框架

	- Python Web框架
	- 结合数据分析、数据库等
	- 可视化组件

		- API原生组件

			- 文字
			- 侧边栏
			- 提示
			- 文件上传下载
			- 表格
			- 下拉框 多选框
			- 滑块 区间滑块
			- 输入框
			- 媒体（音、图、视频）
			- 缓存 性能

		- Components

			- Echarts
			- 3D mol
			- 媒体

- CSV文件、XML文件

	- CSV批量处理，自动建库建表
	- OPC UA 信息模型XML文件自动生成

- 爬虫，浏览器模拟操作
- Instapaper Bookmark

	- 自动同步到OneNote

- PyQt

	- 高温搬运机器人控制程序

### NodeRed

- S7
- OPC UA
- MQTT
- 可视化界面
- Docker

### 协议转换

- MQTT

	- Python SDK

		- 同步
		- 异步

	- QoS
	- SparkPlug B规范

		- 互操作
		- 可discover tags

	- MQTT  over QUIC

		- EMQX 5.0

- HTTP

	- Flask RESTful

		- WebHook
		- Flask2.0
		- TDengine RESTful二次封装

			- 实时数据
			- 近期数据
			- 指定时间段数据
			- OEE计算

- OPC UA

	- SDK

		- Clinet
		- Server

### EMQ消息中间件

- EMQ X Broker

	- Dashboard

		- 5.0 UI、逻辑更新

	- 规则引擎

		- 数据转发
		- 数据集成

			- Webhook 

				- TDengine

			- 商业版kafaka、CH等

		- 消息桥接

			- MQTT桥接

		- 分析计算
		- New可视化流程图

	- Sparkplug B
	- Docker

- MQTTX客户端
- EMQ Neuron（商业收费）

	- 2.0架构开源

		- Docker容器化
		- 管理Web GUI
		- 驱动二进制so文件
		- 配置文件json

- EMQ X Cloud

### 数据存储

- 关系型数据库

	- MySQL

		- SQL
		- Python库
		- 游标、执行
		- Docker

- MongoDB

	- 日志存储
	- 文件存储
	- 也支持IoT时序数据
	- Mongo Chart可视化

- HTAP数据库

	- PingCAP

		- TiDB

			- 场景
			- 工具

				- 安装部署

					- TiUP
					- TiOperator

				- 运维和可视化

					- TiDB Dashboard

				- 数据流转

					- 与TDengine结合

				- 集群灾备

			- 云原生分布式

- Kyligence
- 时序数据库

	- InfluxData

		- Telegraf收集器

			- MQTT
			- OPC UA

		- InfluxDB

			- Docker

		- Chronograf
		- Kapacitor

	- TDengine

		- RESTul接口
		- 类似SQL语法

			- 不等于SQL

		- 统计计算、降维、聚合、滑动窗口
		- 超级表

			- 1个采集点1个Table
			- 分布式传感器汇总计算
			- 基于超级表创建子表

				- 第一次写入可自动创建

			- 动态数据
			- 静态数据（TAG）

		- 集群功能开源

			- compose部署
			- k8s部署
			- 集群主从关系

				- 掉线无法写入

		- 配置文件——时区设置、RESful limt设置
		- 数据导入导出

			- taosdump
			- csv

				- 提前建好Table，csv文件只要数据

		- 基于Streamlit和RESTful的可视化查询和导出
		- Docker

	- QuestDB

		- 查询速度是TD的10倍左右
		- 支持PostgreSQL接口

			- Grafana
			- SQLer

		- Docker

	- Apache IoTDB（清华）
	- MatrixDB超融合时序数据库

		- 超融合
		- Web GUI部署和管理

	- HStreamDB

		- （EMQ）

	- ConosDB
	- Prometheus
	- Clickhouse
	- OpenTSDB

- 向量数据库

	- Milvus开源向量数据库

		- 部署

			- K8s平台部署
			- KubeSphere商店部署

		- 应用场景

			- 相似性搜索
			- 诊断

		- Python SDK

- DBRanking、墨天轮数据库排名

### 数据可视化

- Grafana Lab

	- Grafana

		- 配置项

			- 免登录
			- iframe
			- 非认证插件（TD）

		- datasource

			- Mysql
			- influxdb
			- TDengine

				- 插件安装

			- prostgresql

				- QuestDB（PostgreSQL）

			- websocket
			- opcua

		- Live Streaming
		- 可视化

			- Value mapper
			- 报警

				- Alert List

			- 数据单位
			- OEE State TimeLine插件
			- 跨DataSource汇总计算
			- Variable配置 可变参数面板
			- 数据分析插件、AI机器视觉可视化
			- Inspect数据导出csv

		- Docker

- Echarts

	- Pyecharts

		- Flask集成
		- Streamlit集成

	- JS原生

		- 灵活性好、动态关联集成

- Amcharts

	- Amchart Map

- AG Grid
- Elastic Search Kibana

	- Filebeat
	- Machinebeat

- Streamlit

	- 数据可视化查询及导出

- Superset

	- Docker

- HEAVY.AI（原OmniSci ）

### 形成工业互联网数据采集系统技术体系，应用

- 缺顶层的IoT平台、管理系统

	- 参考西门子Industrial Edge

### ThingsBoard

- Dashboard
- Gateway（MQTT）
- Connector架构图
- Docker容器

### Cockpit Web Console服务器管理web gui

### UWB定位系统

### 西门子MindSphere

- IoT1040 2050

### Qingcloud IoT EdgeWize

- 设备监控
- 驱动管理

	- 同时参考Nueron

- 脚本一键部署

### PingCAP

### Keliygence

### Apache Flink

- NiFi

### 批量部署、批量管理

- NVIDIA Fleet
- Rancher Fleet、K3s
- KubeEdge

## 云计算云原生技术

### 云原生定义

- CNCF定义

	- 容器

		- 不止Docker

	- 服务网格
	- 微服务
	- 不可变基础设施
	- 声明式API

### CNCF

- CKA
- Karmada多集群管理工具（华为）
- KubeVela（阿里）
- OpenFunction（青云）FaaS
- 子主题 5

### LF Edge

### Docker

- Dockerfile
- Docker compose

	- 批量部署

		- 数据采集系统一键部署脚本

- docker镜像导入导出commit
- 容器网络

	- volume

		- 文件copy

			- 启动策略

				- 环境变量

- portainer
- Docker buildx多平台镜像
- dfimage导出dockerfile
- 镜像仓库

	- Harbor搭建和使用
(VMWare开源）

		- Harbor镜像列表导出
		- 镜像x86/arm

			- Python IIoT运行环境
			- TDengine

				- 修改配置文件

			- Grafana

				- TD插件
				- 配置文件

			- Java OPC UA Server

	- Docker hub
	- 阿里云个人仓库

### 阿里Dragonfly镜像P2P加速

### Containerd

- CLI命令行

	- Ctr
	- Crictl
	- 官方nerdctl

### Kubernetes容器平台

- K8s部署

	- kubeadm官方
	- 自建资源包
	- KubeSphere
	- KubeboardSpray
	- MiniKube
	- kind(k8s in docker)

- Kubectl命令行
- 2022-8-2通过CKA认证
- 控制面Dashboard

	- KubeSphere

		- UI优秀

			- 应用导向

		- 可插拔软件
		- 支持KubeEdge脚本一键部署
		- 应用商店
		- DevOps流水线
		- WeaveScope
		- 添加自定义仓库

	- KubeBoard

- 应用部署

	- Helm Chart
	- Operator

### Serverless

- FaaS+BaaS
- 一种服务模式
- CNCF的全景图

	- serverless dev
	- serverless frame
	- 阿里云FC

		- Flask

	- 腾讯
	- AWS Lamda
	- OpenFunction
	- KNative
	- Dapr

### SUSE

- Rancher Lab

	- Rancher
	- Fleet
	- k3s

		- Autok3s

	- k3OS
	- Octopus 

		- 已暂停维护

- SUSE Server软件

	- 服务器
	- Micro OS Edge管理
	- Harvester开源超融合

		- 基于k8s

### 微服务

- Istio

	- Bookinfo Demo

- 微软Dapr

	- v1.0

		- v1.5

	- 微服务
	- 可观测性
	- 分部式运行时
	- SDK

		- Python Flask Demo

	- VS Code插件

- SpringCloud

### 云原生对象存储

- MinIO开源

### 虚拟机管理平台

- VMWare ESXi
- OpenStack

	- Kolla-ansible
	- OpenStack命令行
	- 2022-3-30 Yoga版本

- QingCloud KSV虚拟化
- 超融合系统

	- SUSE Harvester
	- VMWare超融合
	- SmartX

- 服务器

	- 联想服务器

		- 管理口

	- DELL EMC服务器

### 边缘计算框架(k8s衍生)

- 华为KubeEdge

	- keadm部署

		- cloud/edge

	- KubeSphere做控制面

		- 边缘设备远程集中管理、监控、部署

	- Mapper设备管理

		- OPC UA
		- ONVIF

	- EdgeMesh云边通道

- Rancher

	- K3s

		- Autok3s

			- 阿里云等公有云
			- 私有云平台集群导入
			- 自家HCI-Harvester平台

		- K3s与k8s

			- K3s与KubeEdge区别

	- Rancher Desktop

- 腾讯SuperEdge

	- 云端控制面在腾讯云
	- 边缘集群与k8s一键转换

- 阿里OpenYurt

	- 边缘集群与k8s一键转换
	- OpenYurt体验中心

		- 开源Dashboard控制面

- 百度Baetyl(原OpenEdge)
- VMWare

	- EdgeX

		- docker-compose部署
		- v2.0 k8s部署

	- Harbor

		- Docker-compose离线部署

- Micro k8s

	- (Ubuntu)

- 试用、总结PPT、对比表格
- 边无际Shifu IoT框架

	- k8s CRD

		- 设备抽象成Pod

			- OPC UA

				- 转HTTP协议

			- S7

		- 可以与KubeEdge、OpenYurt结合

### 公有云

- 阿里云

	- ECS

		- X86实例
		- ARM实例
		- GPU实例

	- EKA（k8s）
	- 镜像仓库
	- 域名

		- ssl证书

			- 二级域名
			- CName

	- IOT

		- DataV大屏

			- OEE

	- OpenYurt
	- FaaS函数计算

- 腾讯云

	- 实例
	- SuperEdge
	- Serverless国内版-部署

- 百度智能云

	- API
	- Baetyl

- AWS

	- EC2
	- S3
	- greengress
	- iot
	- 认证解决方案架构师（助理级）

- 华为云

	- IoT
	- 工业互联网平台

- Azure

## 人工智能 机器学习

### Pytorch

### TensorFlow

### KubeML

## Vuepress

## GitOps

## 项目

### 内部

- 院内设备数据采集
- 南通二期设备数据采集

### 集团

- 云边协同
- 成飞

## 智能制造

### 工业4.0

### 自动化

### 工业互联网IIoT

### 智能制造成熟度评价

- 技术

	- 数据
	- 集成
	- 信息安全

- 资源

	- 装备
	- 网络

- 航空智能制造成熟度模型

### 信息化系统

- ERP
- MES
- PLM
- 管控系统

### 数字孪生

### 信息物理系统CPS

### 工业5G

- Wifi 6

## 其它

### GitHub

### 软著

- 数据采集软件
- 云边协同MySQL同步
- 时序数据可视化查询
- 自动建库建表
- OPC UA 信息模型XML

### 论文

- EI会议1篇

### 行业协会

- 信通院
- 工业互联网产业联盟
- 边缘计算产业联盟

### 行业交流

- 西门子数字化展厅
- 西门子数控研究中心
- 西门子数控南京工厂

### 分析机构

- Gartner
- 爱分析

### VMware

- EdgeX
- Harbor
- ESXi

### 标杆企业

- 海尔卡奥斯
- 航天云网
- 三一 树根互联
- 徐工信息
- 美的智云
- 寄云科技
- 天泽智云
- PTC thingworx kepware
- 杉数科技
- GE
- 西门子MindSphere
- 研华边缘计算
- ……

### Jimmy Song 宋净超 k8s

### 神农 边缘计算

### 持续的自我驱动力，
发现问题解决问题

### 体系化思维，前瞻性

### 统筹项目管理能力

### 航空航天制造新技术与应用在线会议

