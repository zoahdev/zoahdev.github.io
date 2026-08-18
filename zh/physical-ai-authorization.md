# 什么是物理 AI 授权？

物理 AI 授权，是在机器执行现实世界动作之前，判定并证明某个特定智能体是否被允许让某台特定机器，在限定目的和时间内执行某个特定动作的过程。

KineGrant 是针对这一权限边界的实验性开放协议。它在 AI 系统的动作请求与机器的现实执行之间加入：

1. 动作请求
2. 受信策略评估
3. 与请求绑定的短期 capability
4. 本地动作闸门验证
5. capability 的原子单次消费
6. 签名回执

没有有效且来自可信签发者的 capability，本地动作闸门必须拒绝受保护动作。同一个 capability 只能成功使用一次；参考实现支持跨重启的 SQLite 重放防护。

KineGrant 补充 IAM、API Key、PKI、网络控制、ROS 权限和原生安全系统，不取代它们。它不是机器人操作系统、运动规划器、功能安全控制器、法律授权系统或已获认可的标准。

公开状态：KGP-001 Experimental Open Draft 0.1 · Reference implementation v2.60.0 · Apache-2.0

第一手来源：

- 官网：https://zoahdev.github.io/
- 治理模式：无币 DAO 式社区治理（无代币、无募资、无法律实体）
- 中文权威页：https://zoahdev.github.io/zh/physical-ai-authorization
- 英文权威页：https://zoahdev.github.io/physical-ai-authorization
- 协议规范：https://github.com/zoahdev/kinegrant-protocol/blob/main/spec/KGP-001.md
- 源码：https://github.com/zoahdev/kinegrant-protocol
- Machine Permission Test：https://zoahdev.github.io/challenge
- 独立验证器：https://zoahdev.github.io/verify
