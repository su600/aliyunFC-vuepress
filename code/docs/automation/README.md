# 自动化技术

自动化的技术背景，PLC、控制系统、传感器、各类设备

各种现场总线、协议、通讯、OPC UA、MQTT

形成数据采集的需求及其解决方案，以开源、Python为主

随后不断与云原生相关技术元素结合，比如Docker，借鉴云原生生态、行业的一般方案，应用于工业

本质是以云原生的思想和解决方案来解决工业互联网问题。

## 工业互联网数据采集解决方案

### 基于Python的协议转换

- pyads
- pylogix
- pymodbus
- opcua
- focas

---

### NodeRed

最早是MICA上看到的，支持s7、OPC UA等采集协议，带有Web界面，MQTT，编程快捷简单

- 模块化系统采集与控制
- 工业互联网演示系统OPC UA集成互操作
- UR机器人
- 现在依然使用、很方便

### EMQX

emqx

- 规则引擎
- Neuron网关（2.0开源）

### 时序数据库（TDengine为主）

sss

- TDengine
- IoTDB
- MarixDB
- 其它数据库比如TiDB等归在云原生技术领域

### 数据可视化（Grafana为主）

sss

- Grafana
- ThingsBoard
- Elastic Search的Kibana

### RESTful

sss

基于flask-restful对TDengine的RESTful接口进行二次封装

### OPC UA

- Server
- Client

---
