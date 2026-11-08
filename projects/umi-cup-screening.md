# UMI Arena 杯子任务数据筛选与模型实验

领域：具身学习与数据质量
证据状态：已有公开方法仓库与聚合结果

按 episode 筛选成功杯子演示，保留可逆隔离视图与人工/机器证据层，并记录后续模型实验。

## 实现与产物

- 3975 episodes / 827323 frames 输入
- 3423 episodes / 746914 frames 保留
- 552 episodes / 80409 frames 隔离
- machine 551、人工标记 14、重叠 13，union 552

## 证据

- 已有公开仓库 README 的 aggregate result
- 公开方法包还记录 π0.5 / OpenWAM 训练及三相机仿真实验进展

## 当前边界

- 聚合值来自已有公开仓库；本机没有原始数据，未重新运行筛选
- 筛选结果不是机器人连续 IK、碰撞或动力学可行性证明
- 受限 AIRoA 数据、逐 episode 报告、视频、selection manifest 与模型不随汇总公开
- 不宣称完整杯子任务成功已确认

## 代码与来源

- https://github.com/zc1q84zc-boop/umi-arena-cup-screening-methods

[返回成果总览](../README.md)
