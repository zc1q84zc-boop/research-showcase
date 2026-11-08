# PiPER RGB-D 抓取与 Pink 规划流水线

领域：机器人操作
证据状态：已有抓取计划与多次 episode 输出；成功率未汇总

连接 D405、四类 YOLO、GraspGenX 与 Pink，形成检测、点云、抓取候选、IK、碰撞检查及受控执行流程。

## 实现与产物

- GraspGenX 独立 ZMQ 服务
- 目标 mask 清理与背景点云分离
- 手掌、手指、相机、机械臂 proxy 检查
- plan.json、碰撞场景与候选阶段间距日志

## 证据

- real_piper/README.md
- outputs/ 下至少 3 份 plan.json 以及 episodes/ 多次实验目录

## 当前边界

- 输出目录存在不证明抓取成功
- 观测点云过滤可能忽略小/薄障碍物；部分配置不做 lift path 碰撞门控
- 工作区几何尚未完成验证；不声称完整自主实机系统已验收
- GraspGenX 与 Pink 为上游技术，个人贡献不作未经核实的归属判断

## 代码与来源

- https://github.com/JizhuoChen/real_piper
- https://github.com/NVlabs/GraspGenX

[返回成果总览](../README.md)
