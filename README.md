# [Cortex](https://doc.soc.xin/architecture/index.html)

[![Build Status](https://github.com/SoCXin/Cortex/workflows/docs/badge.svg)](https://github.com/SoCXin/Cortex)


[Cortex](https://doc.soc.xin/architecture/arm.html) 是 [ARM(Advanced RISC Machine)](https://www.arm.com/) 公司一个处理器系列，在Classic系列最后一代ARM11系列后推出，首代基于ARMv7架构。

* Cortex-M
    * [Cortex-M0](https://www.soc.xin/Cortex-M0)
* Cortex-R
* Cortex-A
* Cortex-X


Cortex-M系列基于ARMv7-M架构（用于Cortex-M3和Cortex-M4）构建，而较低的Cortex-M0+基于ARMv6-M架构构建。首款Cortex-M处理器于2004年发布，当一些主流MCU供应商选择这款内核，并开始生产MCU器件后，Cortex-M处理器迅速受到市场青睐。可以肯定的说，Cortex-M之于32位MCU就如同8051之于8位MCU——受到众多供应商支持的工业标准内核，各家供应商采用该内核加之自己特别的开发，在市场中提供差异化产品。例如，Cortex-M系列能够实现在FPGA中作为软核来用，但更常见的用法是作为集成了存储器、时钟和外设的MCU。在该系列产品中，有些产品专注最佳能效、有些专注最高性能、而有些产品则专门应用于诸如智能电表这样的细分市场。

Cortex-R面向实时应用的高性能内核，多数实时处理器不支持MMU，不过通常具有MPU、Cache和其他针对工业应用设计的存储器功能。实时处理器运行在比较高的时钟频率（例如200MHz 到 >1GHz ），响应延迟非常低。虽然实时处理器不能运行完整版本的Linux和Windows操作系统， 但是支持大量的实时操作系统（RTOS）。

Cortex-A (Application Processors)这类处理器运行在很高的时钟频率（超过1GHz），支持像Linux，Android，MS Windows和移动操作系统等完整操作系统需要的内存管理单元（MMU）。

2020年05月发布的Cortex-A78要兼顾性能、功耗、面积不同所有提升有限，同时推出首款专注于高性能的Cortex-X系列核心Cortex-X1，相较A78整数性能提升了22%。

2021年3月底，Arm正式发布了全新的Armv9指令集。

2021年更新 Cortex-X2 的整数性能相比 Cortex-X1 提升了 16%。对应的中核Cortex-A710(A78继任)和小核Cortex-A510(A55继任)，均基于 Armv9 兼容设计。

2022年更新 Cortex-X3在架构设计上的变化相当深入、广泛，比如解码器每周期指令从5个增加到6个，乱序执行窗口从288个增加到320个， ALU整数算数单元从4个增加到6个，二级缓存容量从512KB翻番到1MB，并且不再支持32位指令集。
对应中核 Cortex-A715 注重性能与能效的平衡，对比Cortex-A710在同等性能下能效提升最多20％，而在同等功耗下性能提升最多5％。已经达到Cortex-X1的性能水准。

性能方面，3.3GHz频率、1MB二级缓存、8MB三级缓存的配置下，与基于Cortex-X2的安卓旗舰处理器对比，提升最多25％。3.6GHz频率、1MB二级缓存、16MB三级缓存的配置下，与主流笔记本处理器(Intel i7-1260p)相比，单核性能高出最多34％。
