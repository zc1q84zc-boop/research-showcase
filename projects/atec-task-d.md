# ATEC Task D：B2PiPER 推箱与越障提交

领域：竞赛仿真
证据状态：多个提交方案已存档；成绩未独立核实

提交目录包含严格在线策略命令序列、攀爬策略切换以及历史动作回放版本。

## 实现与产物

- 在线方案从 proprio 构造策略观测
- 120 steps settle 后推箱，再切换 climb policy
- current_score 用于完成早停
- 保留 online 与 action replay 方案差异

## 证据

- Clear_ATEC2026_Simulation_Challenge/submissions/TaskD/README.md
- submissions/ 下保留多种 Task D 提交目录

## 当前边界

- 未找到可用的该版本完整评测视频或统一成绩表
- 命令序列通过策略在线推理，与固定关节动作回放必须区分
- 不声称获奖、官方成绩或跨 seed 泛化

## 代码与来源

- https://github.com/StevenLiudw/Clear_ATEC2026_Simulation_Challenge

[返回成果总览](../README.md)
