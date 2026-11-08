# ATEC Task E：PiPER 桌面操作流水线

领域：竞赛仿真
证据状态：多种 baseline 与在线提交接口已存档

探索 ACT、Cartesian/cuRobo、启发式物理与成功动作 profile 的在线适配。

## 实现与产物

- RGB-D 目标中心估计
- 依据 current_score 推进目标顺序
- 成功 profile 选择、插值与备用重试
- Docker/server/solution 提交结构

## 证据

- submissions/task_e_online_curobo_pipeline_root_submission/README.md
- submissions/ 中 ACT、cuRobo、heuristic 与 replay 版本并存

## 当前边界

- README 中 seed-120/130 full-success 为已有说明的陈述，本次没有复核对应完整原始评测
- 在线接口保留 profile 驱动，不能描述成每步完整重跑 SAM/AnyGrasp/cuRobo
- 不以官方 baseline.gif 作为个人实验成果

## 代码与来源

- https://github.com/StevenLiudw/Clear_ATEC2026_Simulation_Challenge

[返回成果总览](../README.md)
