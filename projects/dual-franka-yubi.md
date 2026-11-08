# 双 Franka + YUBI Isaac Sim 环境

领域：双臂操作与仿真
证据状态：已有公开环境与策略/录像接口

双 Franka Panda、YUBI 夹爪、杯盘桌面场景，支持可复现随机布局、三相机、策略接口和同步记录。

## 实现与产物

- reset/step API 与 state/image 观测
- 关节目标与末端轨迹策略 hook
- 有界 differential IK
- MP4、关节 CSV、manifest/report 同步记录

## 证据

- 已有公开 dual-franka-yubi-isaac-sim README 与源代码
- 环境描述包含 Isaac Sim 5.1、相机与资产审计说明

## 当前边界

- 本次未在本机启动 GPU 仿真或复核物理运行
- 几何、质量、摩擦与相机参数含估计值；环境完成不等于真实任务迁移成功
- NVIDIA Panda 资产依赖需用户合法本地提供；YUBI CAD 保留上游许可

## 代码与来源

- https://github.com/zc1q84zc-boop/dual-franka-yubi-isaac-sim

[返回成果总览](../README.md)
