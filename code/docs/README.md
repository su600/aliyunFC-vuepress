# My VuePress WebSite🚀️ 

这是我的VuePress WebSite，代码托管在GitHub上，以Serverless形式托管在阿里云FC上

- 1
- 2
- 3

---

- [ ] 好的
- [ ] 测试
- [ ] 域名绑定
- [ ] 证书申请 v.su600.cn

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from fbprophet import Prophet

data = pd.read_excel('./xxx.xlsx')
data['date'] = pd.to_datetime(data['date'], format='%Y%m%d')
data = data.rename(columns = {"date":"ds", "y":"y"})[["ds","y"]]
data.head(5) #查看前五条记录
data.tail(5) #查看后五条记录

# 模型保存
with open('prophet_model.json', 'w') as md:
    json.dump(model_to_json(model), md)

# 模型读取
with open('prophet_model.json', 'r') as md:
    model = model_from_json(json.load(md))
```

## 好的 这是二级标题

## 也是❤️ 

### 这是三级标题测试

> 这是引用文字
