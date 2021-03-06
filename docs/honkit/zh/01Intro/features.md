# 功能总览

Kubean 功能特性包括但不限于：

- 支持集群生命周期管理，包括集群的创建、升级和删除，确保集群升级期间不会影响业务
  - 支持一键创建集群，能够应对私有云虚拟化场景，对于物理机将给出 IP 和登录凭证
  - 集群升级，支持 Kubernetes 连续大版本升级，使应用向下兼容
  - 集群删除
  - 一键轮滚证书
  - 详尽的安装/运维日志
- 支持节点生命周期管理
  - 在线和离线新增节点
  - 删除节点
  - 节点污点管理
  - 节点标签管理
  - 支持丰富的容器运行时接口（CRI）
    - containerd
    - docker
    - runc
    - docker
    - kata
    - gvisor
- 集群检查：安装前、安装后
- 集群组件高可用
  - 单台 master 节点宕机不影响集群正常使用
  - 管理节点故障后，集群运行状态不受影响，业务正常使用
  - 容器管理平台节点故障，可自动弹探测、切换，不影响平台自身的对外提供服务

