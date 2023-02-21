# operator-demo
kubebuilder 演示demo

# 目录
- 1-下载kuberbuilder
- 2-创建目录
- 3-初始话项目
- 4-模型及控制器
- 5-添加证书服务器
- 6-添加webhook
- 7-打包测试

# 下载kuberbuilder
- 官方网址[https://book.kubebuilder.io/]
- git 仓库地址[https://github.com/kubernetes-sigs/kubebuilder]
## 安装执行脚本

```shell
curl -L -o kubebuilder https://go.kubebuilder.io/dl/latest/$(go env GOOS)/$(go env GOARCH)
chmod +x kubebuilder && mv kubebuilder /usr/local/bin/
```

# 创建目录
```shell
mkdir <PROJECT_DIR> && cd <PROJECT_DIR>
```

# 初始化项目-模型及控制器

## 一键初始化
```shell
kubebuilder init --domain ljtian.com
```
## 检查项目信息
```shell
cat PROJECT
```

## 创建API
```shell
kubebuilder create api --group apps --version v1 --kind MyDaemonset
```