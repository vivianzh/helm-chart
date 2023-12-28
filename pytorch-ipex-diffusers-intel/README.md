#pytorch-ipex-diffusers-intel v0.1.0
### Optional: Chart parameters

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

