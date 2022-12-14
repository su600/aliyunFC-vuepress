# 个人技术体系🚀️
code.su600.cn

这是我的VuePress WebSite，梳理一下主要技术点，便于查看和随时修改。

以终为始的寻找差距，以当前能力范围探寻价值

- 代码托管在GitHub的Vuepress仓库里
- 服务以Serverless形式托管在阿里云FC上 (免费)
- 二级域名 v.su600.cn 已添加证书

---

个人是以自动化、测控技术为教育背景，有一定的工业自动化技术基础。从硕士阶段关注、学习云计算相关技术和应用。

工作前几年以智能制造、工业4.0、IoT、工业互联网为主要研究和学习方向，同时逐步扩展融合边缘计算、云计算、云原生技术领域，随技术和生态发展，两大技术体系越来越融合。个人技术体系的主要分类：

1. 工业自动化基础
2. 工业通讯、工业4.0基础、智能制造
3. 工业互联网设备数据采集
4. 编程语言 Python Golang
5. 协议转换
6. EMQX相关产品生态 MQTT
7. 数据库相关技术和产品 时序数据库
8. 数据可视化技术和产品
9. 云原生基础
10. 容器技术（Docker）
11. Kubernetes、KubeSphere，2022年通过CKA认证
12. 超融合平台
13. 微服务技术 Istio
14. 虚拟机平台
15. 云原生边缘计算框架
16. 公有云相关技术和产品
17. Serverless
18. Infrastructure as Code-Terraform
19. 主要项目和解决方案
20. 参观、参会记录
21. 关注的组织、行业协会、信通院、行业交流、分析咨询机构
22. 工业互联网头部企业
23. 白皮书技术资料等
24. 智能制造成熟度诊断

## 这是代码高亮测试：

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from fbprophet import Prophetdata = pd.read_excel('./xxx.xlsx')
data['date'] = pd.to_datetime(data['date'], format='%Y%m%d')
data = data.rename(columns = {"date":"ds", "y":"y"})[["ds","y"]]
data.head(5) #查看前五条记录
data.tail(5) #查看后五条记录
```

# 模型保存

```python
with open('prophet_model.json', 'w') as md:
    json.dump(model_to_json(model), md)
```

# 模型读取

```python
with open('prophet_model.json', 'r') as md:
    model = model_from_json(json.load(md))> 
```

> 这是引用文字
