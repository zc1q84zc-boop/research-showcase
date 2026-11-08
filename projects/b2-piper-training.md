# B2 + PiPER 运动策略训练与可迁移交付包

领域：强化学习与移动操作
证据状态：已形成训练交付；楼梯增强目标未验收

保留 actor-only warm start、critic warmup、分阶段课程、确定性评估和带哈希的跨机器交付。

## 实现与产物

- 45 actor / 251 critic / 12 leg actions，20 ms 周期
- 安全重复摆腿与后腿高度增量奖励
- flat unlock → low speed → full range 课程
- canary、平地及楼梯筛查工具与 provenance

## 证据

- 桌面/B2_Piper_policy_transfer_20260821/训练部署说明
- 源码 bundle、覆盖补丁、checkpoint 与 flat/stairs evidence 目录存在
- 桌面/b2_piper_omni_training_bundle_20260818/ 作为较早交付版本

## 当前边界

- model34 被文档定义为失败对照，不可写为成功楼梯策略
- SafeRearSwingHeightIncrement 在交付时尚未训练验证
- stairs_specialist 在该说明中仍是待实现工作

[返回成果总览](../README.md)
