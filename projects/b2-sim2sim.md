# B2 MuJoCo 策略验证与地形 Demo

领域：四足运动控制
证据状态：已有录像与六场景仿真结果

将 Unitree B2 ONNX 策略封装成独立 MuJoCo 交互和批量评测工具，覆盖平地、转向、坡道、楼梯及粗糙地形。

## 实现与产物

- 键盘速度控制与实时 viewer
- 观测/动作、关节顺序、PD 控制合同核对
- 视频、轨迹与 JSON 结果可追溯
- 仿真与实机 shadow/诊断入口分离

## 证据

- 2026-08-12 smoke：6/6 completed，6 provisional passes，0 falls
- 平地 0.5 m/s 指令：8 s 计分窗口前进 3.3534 m，速度 RMSE 0.08118 m/s
- 6 段公开 Demo 与精简机器可读评测已随本仓库收录

## 当前边界

- provisional_pass 是该次评测规则下的暂定通过，不代表统计稳定性、通用越障或实机成功
- 楼梯录像不自动等同 course_complete
- 该仓库 2026-08-12 实机记录在初始化阶段受阻，policy_steps=0；后续控制台硬件日志需分开评价

## 代码与来源

- https://github.com/StevenLiudw/B2_sim2real

## 原项目入口示例

需要原项目及其依赖；这些命令未在本次盘点重新执行。

```bash
python -m sim2sim_b2.run_interactive --policy models/policy.onnx
```

[返回成果总览](../README.md)
