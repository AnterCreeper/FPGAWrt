# Open SmartRouter with OpenWrt

This Project is under **Work-In-Progress** now  
**该项目还未完善**

If any questions, welcome for Issues & PRs   
如果有疑问，欢迎提交Issues或PR

**WARNING! This Project is not been fully productive tested, use at your own risk!**   
**警告！该项目未经充分的生产测试，使用需要你自己衡量**

### License

This project is licensed under the LGPL-2.1-or-later license. **DO NOT** download or clone this project until you have read and agree the LICENSE.     
该项目采用 `LGPL-2.1 以及之后版本` 授权。当你下载或克隆项目时，默认已经阅读并同意该协定。

### Overview

This project is an **Open Source** platform of Programmable SmartRouter based on Xilinx Kria K26 SoM, takes **OpenWrt** Operating System and aimed for providing an ***easy-to-use*** and ***low-cost*** platform for `Network System` exploration and research.  
Related works doesn't contains General Purpose Processor which makes it hard to use in productive SOHO and Consumer environment. Besides, `Zynq Ultrascale+` would provide more features such as `Cache Coherence` and `Video Codec`.  

该项目是基于 Xilinx Kria K26 系统模块构建的**开源**可编程智能路由器, 搭载 **OpenWrt** 系统, 旨在提供一个***易于使用***和***廉价***的`网络体系`探索和研究平台。  
类似的工作通常由纯 FPGA 构建不包含通用处理器, 因此缺乏 SOHO 和消费级环境的实用性。此外, `Zynq Ultrascale+`可以提供更多功能, 例如`缓存一致性`和`视频编解码`等。

This project consists of:
- Kicad PCB project
- FPGA RTL and Cortex-R5F firmware
- P4 compiler, Net Processor compiler
- DPDK and VFIO drivers
- Custom OpenWrt packages

该工程包含:
- Kicad 印刷电路板工程
- FPGA RTL 代码, 以及实时核心固件
- P4 语言编译器, 网络处理器编译器
- DPDK 和 VFIO 驱动
- OpenWrt 软件包

### Params of K26 SoM
- Quad-core Arm Cortex-A53 @1.5 GHz, support Virtual Machine
- Dual-core Arm Cortex-R5F @600 MHz
- 1x VCU, support H.264 and H.265 decode/encode
- 4GBytes 64-bit(non-ECC) DDR4 @2400MT/s
- 16GiB eMMC
- ARM SMMU and CCI-400, support IOMMU and CC(Cache Coherence) for PL

### Params of Carrier Board
- 4x 10G SFP
- 1x m.2(PCIe 2.0 x4, 4GB/s max) for NVME or SATA HBA
- 1x GBE + 1x 2.4GHz Wireless(ESP8089) for Management
- 1x microSD
- 1x USB 2.0
- 1x USB-C for Power(PD), 1x USB-C for Debug
