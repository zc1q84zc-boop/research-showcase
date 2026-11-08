# OdinEye P1A：几何条件 BEV 感知

领域：视觉与空间感知
证据状态：源码与技术说明已存档；本次未复跑训练

RGB 历史与标定相机高度，经冻结 VGGT-Ω 和运行时几何构建器，生成当前帧及历史融合 BEV。

## 实现与产物

- 共享一次 VGGT 前向；几何条件解码
- 512×512 单帧与 800×800 融合输出
- 视场外 unknown；证据置信度与几何质量门控
- 直接观测与遮挡补全分区监督，direct-priority PCGrad

## 证据

- VggtBev/README.md；src/ 与 configs/ 存在

## 当前边界

- 未找到本机 runs/artifacts 成果文件，不能据技术说明声称训练完成或精度达标
- 骨干、权重及训练数据不随汇总发布

## 代码与来源

- https://github.com/cicaburnwood-crypto/VggtBev

## 原项目入口示例

需要原项目及其依赖；这些命令未在本次盘点重新执行。

```bash
odineye-p1a-train --config configs/p1a_local_smoke.toml --data-only
```

[返回成果总览](../README.md)
