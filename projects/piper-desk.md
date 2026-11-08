# PiPER Desk 与 VLA Rollout 采集控制台

领域：科研工程与数据采集
证据状态：本机源码与可迁移打包材料已存档

基于 SocketCAN 的机械臂本地网页遥操作和 VLA rollout 采集入口。

## 实现与产物

- 遥测与只读启动
- 手柄 Cartesian 输入、限速与平滑目标流
- PiPER Desk 保持唯一 CAN 所有权
- D405、任务 prompt、dataset 路径、采集频率及 episode 保存界面

## 证据

- Documents/Codex/2026-08-26/help-install-the-piper-sdk-on/README.md
- 桌面/PiPER-VLA-Console-20260917.tar.gz 与 SHA256 文件

## 当前边界

- 采集器实现不代表已完成策略训练或达到任务成功率
- 本次未连接 CAN、相机或执行运动
- 归档源码未随本汇总整体重新公开

## 原项目入口示例

需要原项目及其依赖；这些命令未在本次盘点重新执行。

```bash
./start-teleop.sh
```

[返回成果总览](../README.md)
