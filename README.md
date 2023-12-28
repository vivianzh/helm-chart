# helm-chart

## helm的chart仓库地址为：https://vivianzh.github.io/helm-chart

## 使用方法

1、添加chart仓库 add a chart repository
```
# helm repo add myrepo https://vivianzh.github.io/helm-chart
```

2、添加成功
```
# helm repo list
NAME  	URL
myrepo	https://vivianzh.github.io/helm-chart
```

3、搜索
```
# helm search repo
NAME                              	CHART VERSION	APP VERSION	DESCRIPTION
myrepo/pytorch-ipex-diffusers-intel     0.1.0           0.1.0           A Helm chart for pytorch-ipex-diffusers-intel

```

4、安装
```
# helm install xxx myrepo/pytorch-ipex-diffusers-intel
```
