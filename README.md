# PCIe 互联下 Host/Device 内存共享访问综述

整理 PCIe 的基本访存能力，以及这些能力在昇腾 CANN 的 PCIe Through 和卡间 P2P 场景中的应用。文档使用中文，包含数据流示意图、配置说明与参考资料。

## 阅读文档

- [Markdown 源文档](PCIe互联下Host与Device内存共享访问综述.md)：适合在线阅读和持续修改，图示使用 Mermaid。
- [PDF 阅读版](output/pdf/PCIe互联下Host与Device内存共享访问综述.pdf)：当前共 24 页，包含 17 张图示，适合下载阅读。

## 当前内容

### 第一章：PCIe 基本能力介绍

- Bus Master DMA、PCIe BAR、TX-ATU 与 RX-ATU。
- PCIe P2P 的概念、拓扑、路由与地址映射。
- Host 与 Device 间的 DMA 搬运和直接共享访问。
- 多端点之间的 P2P DMA、共享内存和同步。
- 软件操作、DMA 引擎与 PCIe 内存事务之间的关系。

### 第二章：PCIe 基本能力在昇腾上的应用

- Device 通过 PCIe Through 直接访问 Host 内存。
- 设备访存地址如何路由到 PCIe 出站路径。
- PCIe 组网下的卡间 P2P 拷贝与共享访问。
- CANN 接口、资源生命周期与同步要求。

## 维护方式

以 Markdown 为内容源文件；内容更新后重新导出 PDF，并同步更新阅读版。PDF 中的图示布局可能为适应纸张宽度而调整。具体产品支持范围、接口约束及硬件实现，以正文引用的官方资料为准。
