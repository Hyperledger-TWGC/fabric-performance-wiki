# TWGC Fabric 性能优化小组 wiki

TWGC Fabric 性能优化小组 wiki

TWGC Fabric Performance Special Interest Group wiki

# 项目介绍

随着 Fabric 的使用已经越来越广泛，Fabric 性能问题也日益凸显，为了更好的研究和优化 Fabric 性能问题，2020年7月13日，TWGC 成立了性能优化小组以便为大家提供优化方案和参考实现。

目前 TWGC 性能优化小组主要研究方向：

1. Fabric 性能问题

    主要从两个方面探索Fabric性能的优化方案：Fabric 项目自身性能和 Fabric 应用系统架构设计。我们通过 Fabric 性能优化相关论文讨论，社区成员优化经验分享等方式梳理优化思路，目前整理了 Fabric 性能优化 [思维导图](https://www.processon.com/view/link/5f3c06ec7d9c0806d41fec86) ，欢迎大家参考和补充！

2. Fabric 性能测试工具

    我们目前推出了两个 Fabric 开源测试工具：

    - [Tape](https://github.com/guoger/tape)：一个轻量级 Fabric 测试工具，直接使用 gRPC 和 Fabric 网络连接发送交易请求，并利用 Go 语言高并发特性向 Fabric 网络进行压力测试，避免了 SDK 造成的压测工具性能损失。同时，Tape 配置简单，仅需配置相关交易参数和证书即可实现一键启动。目前 Tape 已支持 TLS 双证书、单独压测 Fabric 交易声明周期中提交和背书阶段、交易发送速率控制等功能，Tape 也正在陆续开发新特性，以支持更多场景的 Fabric。欢迎大家试用和贡献！
    
    - [Probe](https://github.com/SamYuan1990/Probe)：用于测试 Fabric 最优网络参数，可根据配置项结合 Fabric 测试网络自动执行网络启停 Fabric 区块链网络，并利用测试工具 Tape 测试 TPS 指标，最终结合前端页面展示网络配置参数之间关系，以及得到最优配置参数，为 Fabric 开发人员提供参考。

## 加入方式

目前小组开放加入，加入 Fabric 性能优化小组可以联系以下人员：

| 姓名   | 微信        | 邮箱                 | GitHub-ID     | 角色     |
| ------ | ----------- | -------------------- | ------------- | -------- |
| 程阳   | yycheng418  | chengyang418@163.com | Stone-ch      | 组长     |
| 袁怿   | oe19901019  | yy19902439@126.com   | SamYuan1990   | 副组长   |
| 许强   | xq_19880125 | xq-310@163.com       | XuHugo        | 副组长   |
| 李明轩 | Lmx-1994    | s380932081@qq.com    | Matthewbalala | 核心成员 |
| 赵世宏 | zshong1987  | 523713078@qq.com     | tianxuanhong  | 核心成员 |

作为 Fabric 性能优化小组的一员，我们更愿意你：
1. 熟悉 Fabric 源码或应用开发；
2. 有 Fabric 或其他系统性能分析、优化经验；
3. 愿意持续为 Hyperledger 开源社区做贡献。

## 例会信息

每周二晚 21:00-22:00，会议记录保存在小组资料库中。会议记录会同步在wiki中，会议录屏保存在百度云盘。



百度网盘链接: https://pan.baidu.com/s/1XcVS5kY4BfxQUxybyJF_wA 提取码: h38i 



腾讯会议链接：https://meeting.tencent.com/s/lfnnPoSz5JTE

会议 ID：437 1864 9713



所有小组成员在开始会议前可以将自己的议题更新到“资料库->会议记录->当前日期”对应的文档中，我们将预留时间在例会中进行讨论。
