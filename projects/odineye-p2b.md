# OdinEye P2B：双专家与尺度 Token

领域：视觉与空间感知
证据状态：实验实现已存档；效果待核验

冻结 VGGT token memory 后，Observed、Guessed 与 Routing 路径处理直接观测和遮挡补全，并学习米制尺度。

## 实现与产物

- P2B-NLL：Beta evidence 与 evidential NLL
- P2B-BCE：Bernoulli 分类确定性
- RGB-only 推理与 6.5 m / 10 m BEV 合同
- 单次骨干提取；专家路径分离

## 证据

- VggtBev-worktrees/p1b-bce/README.md；当前说明明确区分 P2B 与 legacy P1B

## 当前边界

- BCE 置信度不能表述成认知不确定性
- 没有在本次盘点中核验最终 checkpoint 或验证指标
- 旧 P1B 与新 P2B checkpoint schema 不兼容

## 代码与来源

- https://github.com/cicaburnwood-crypto/VggtBev

## 原项目入口示例

需要原项目及其依赖；这些命令未在本次盘点重新执行。

```bash
python -m vggt_bev_method1.cli_train_p2b --config CONFIG.toml
```

[返回成果总览](../README.md)
