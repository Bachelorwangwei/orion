## 概述

NGC 基础镜像参见
https://docs.nvidia.com/deeplearning/frameworks/pytorch-release-notes/rel_19-09.html#rel_19-09

## 构建镜像

为构建镜像，用户需要将 `install-client-10.1` 放置到当前目录下。

## 验证

假定用户已经成功启动了 Orion Controller 和 Orion Server，并配置好了Orion Client与Orion Server之间的通信模式（SHM/RDMA/TCP)。

在容器中运行

```bash
cd /root/examples/mnist
python main.py
```

即可验证。

## 附

我们已将 [PyTorch官方示例](https://github.com/pytorch/examples) 克隆到`/root/examples`目录下。