# 云计算与云原生

引言

## 该技术线主要发展经历

上学期间参与阿里云在线实践，试用AWS，2016年通过AWS解决方案架构师认证

购买域名su600.cn

一直积极使用公有云，了解技术趋势、产品发展，发挥公有云的巨大便利性。

阿里、腾讯、华为、百度、青云等。

## 主要是公有云的产品

- 阿里ECS、容器加速、镜像仓库、k8s、serverless、oss、域名等、openyurt
- 腾讯serverless、镜像仓库、superedge
- 青云，虚机，镜像仓库，IoT、EdgeWize
- Azure 虚机，关注IoT，time-insight时序数据库

OpenStack相关了解和测试，目前已经凉了，已经有构建在k8s之上的虚拟机解决方案
- 青云 KubeSphere
- SUSE Harvester超融合架构

---

## 云原生技术

最早尝试LXC后直接转Docker，以Docker为基础，Docker容器本身及其衍生生态，然后逐步过渡升级到k8s

k8s是面向一切的、云原生时代的操作系统

- Docker
- k8s
- KubeEdge、SuperEdge、OpenYurt、EdgeX、k3s
- Serverless（更多的是服务模式，并不是全新架构）
- IaC(Terraform) 也是声明式API，用的是公有云本身的开放API能力，聚合封装了一下
- Shifu Framework，持续关注吧，个人感觉一般，局限于HTTP并不高效，且KubeEdge在做DMI接口标准，类似

