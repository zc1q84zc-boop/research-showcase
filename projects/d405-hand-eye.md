# PiPER + D405 ChArUco 手眼标定

领域：机器人标定
证据状态：已有数学质量报告；物理工作区尚待验证

完成眼在手上的相机内参与手眼变换求解，并保留采样筛选及质量阈值。

## 实现与产物

- ChArUco 5×7、30 mm 方格、15 mm 标记
- 23 组原始采样；15 组相机标定、14 组最终手眼求解
- 相机重投影 RMS 0.4730 px
- 手眼平移 RMS 6.5509 mm、旋转 RMS 1.2771°

## 证据

- real_piper/calibration/DELIVERY_README.md
- 通过预设 8 mm / 2° 数学阈值

## 当前边界

- workcell_geometry_verified=false；数学残差不等同独立物理精度
- 不发布相机序列号、原始实验照片或本机配置
- 标定交付说明与后续运行配置可能有时间差异

[返回成果总览](../README.md)
