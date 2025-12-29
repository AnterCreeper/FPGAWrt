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

This project is an **Open Source** platform of Programmable SmartRouter based on Xilinx Kria K26 SoM(Low cost version based on ZYNQ-7000?), aimed for providing an easy-to-use platform for network system exploration and research.

This project consists of:
- Kicad PCB project
- FPGA RTL and Cortex-R5F firmware
- P4 compiler, Net Processor compiler
- DPDK and VFIO drivers
- Custom OpenWrt packages

### Params of K26 SoM
- Quad-core Arm Cortex-A53 @1.5 GHz, support Virtual Machine
- Dual-core Arm Cortex-R5F @600 MHz
- 1x VCU, support H.264 and H.265 decode/encode
- 4GBytes 64-bit(non-ECC) DDR4 @2400MT/s
- 16GiB eMMC
- ARM SMMU and CCI-400, support IOMMU and CC(Cache Coherence) for PL

### Params of Carrier Board
- 4x 10G SFP
- 1x m.2 slot(PCIe 2.0 x4) for NVME or SATA HBA
- 1x GBE + 1x Wifi+BLE(SDIO) for Management
- 1x microSD
- 1x USB 2.0
- 1x DisplayPort(?)
- 1x USB-C for Power(PD), 1x USB-C for Debug
