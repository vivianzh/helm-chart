## helm chart仓库地址为：https://vivianzh.github.io/helm-chart

## 使用方法

1、添加chart仓库
```
# helm repo add myrepo https://vivianzh.github.io/helm-chart
```

2、添加成功
```
# helm repo list
NAME  	URL
myrepo	https://vivianzh.github.io/helm-chart
```

3、搜索chart包
```
# helm search repo
NAME                              	CHART VERSION	APP VERSION	DESCRIPTION
myrepo/pytorch-ipex-diffusers-intel     0.1.0           0.1.0           A Helm chart for pytorch-ipex-diffusers-intel

```

4、安装
```
# helm install xxx myrepo/pytorch-ipex-diffusers-intel
```

以下是目前支持的配置选项和默认值
```
# helm show readme myrepo/pytorch-ipex-diffusers-intel
The table lists the configurable parameters of this chart.

Parameter                      Description                       Default
image.repository               Image repository                  registry.cn-hangzhou.aliyuncs.com/cloudnativeforai/pytorch-ipex-diffusers-intel
image.tag                      Image tag                         devel
image.pullPolicy               Image pull policy                 IfNotPresent
resources.limits.cpu           CPU resource limit                32
resources.limits.memory        Memory resource limit             64Gi
resources.requests.cpu         CPU resource request              32
resources.requests.memory      Memory resource request           64Gi
volumeMountName                the name of the volume            datavolume
volumeMountPath                Mount path                        /data/models
volumeHostPath                 Directory location on host        /data
volumeHostPathType             Directory type                    Directory
hostNetwork                    Whether to use the hostnetwork    false
```

例如：将host目录/mnt/test挂载到/data/models
```
#helm install --set volumeHostPath=/mnt/test xxx  myrepo/pytorch-ipex-diffusers-intel
```
