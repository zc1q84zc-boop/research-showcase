# 四类垃圾实例分割与部署导出

领域：视觉感知
证据状态：v4 有正式训练报告与独立测试集指标

基于 YOLO26s-Seg 进行易拉罐、西瓜皮、纸袋及纸餐盒四类分割。

## 实现与产物

- 1070 张图片、1157 个实例
- 37 个拍摄 session 整组划分
- train/val/test = 643/212/215 张
- PyTorch、ONNX、OpenVINO 导出与代表图加载检查

## 证据

- 2026-08-26 TRAINING_REPORT_V4.md：总体 mask precision 0.936，recall 0.778，mAP50 0.914，mAP50-95 0.792
- 模型推理约 5.9 ms/图，为报告值，不包含完整流水线
- 下载中另有 hybrid v2 和 v7 交付归档，本页指标仅对应 v4

## 当前边界

- 不将 v4 指标套用到 v7 或 hybrid 模型
- session 隔离内部测试不替代新场景视频验收
- 不公开原始训练图像、权重或目标设备 TensorRT engine

[返回成果总览](../README.md)
