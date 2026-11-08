# VGGT Method II：观测区域 BEV 与模拟器对照

领域：视觉与空间感知
证据状态：训练与推理框架已存档；本机权重未核实

由 VGGT 预测深度、内参与相对位姿，经过地面拟合、特征 splatting 与射线证据，预测可见性及可见区域占据。

## 实现与产物

- observed 与 occupancy 双输出
- 累计历史融合；训练和推理共享预测几何
- RGB-only 推理接口与 HTTP runtime server
- Habitat UI 中同步对照 GT 与模型

## 证据

- VggtBev-worktrees/P2/README.md；models/ 中实际仅发现 SHA256SUMS

## 当前边界

- README 描述历史 epoch-10 模型，但本机目录没有对应权重；不能把文档描述视为本机运行验收
- normalized P2 与 legacy metric checkpoint 的尺度、分辨率不同

## 代码与来源

- https://github.com/cicaburnwood-crypto/VggtBev

## 原项目入口示例

需要原项目及其依赖；这些命令未在本次盘点重新执行。

```bash
vggt-bev-infer --model 5m --session SESSION --output-dir OUTPUT
```

[返回成果总览](../README.md)
