# B2 Control Center：统一控制与诊断台

领域：四足运动控制
证据状态：本机代码、仿真录像与硬件诊断日志已存档

统一策略装载、键盘/手柄指令、仿真、LowState 诊断、日志与录屏。

## 实现与产物

- Stack10 423 维输入、50 Hz、10 帧选择性历史适配
- SHA-256 策略合同核对
- 仿真优先与硬件门控
- 网页控制台与目标/实际跟踪统计

## 证据

- b2_control_stack/README.md
- logs/videos/ 有多次平地、草地、泥地与 10–20 cm 台阶实验录像
- logs/control-center/ 有 2026-08-14 至 2026-08-20 的硬件跟踪记录

## 当前边界

- 硬件日志存在不等于稳定落地行走已验收
- 423 维 Stack10 与其他 45 维 actor 属于不同策略合同，不可混用
- 公开仓库与本机副本可能有版本差异

## 代码与来源

- https://github.com/zc1q84zc-boop/b2-control-center

## 原项目入口示例

需要原项目及其依赖；这些命令未在本次盘点重新执行。

```bash
python -m b2_control.cli_control_center --no-open-browser
```

[返回成果总览](../README.md)
