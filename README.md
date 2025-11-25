# 开源智能电动自行车/摩托车（NFC & 蓝牙无钥匙启动版）

本项目致力于打造以**ESP32为主控**，集成**蓝牙BLE**与**NFC无钥匙启动**的智能两轮车控制系统。

## 项目特色
- **NFC无钥匙启动**：支持刷卡/标签身份认证启动
- **蓝牙App远控**：手机App解锁、上锁、启停操作
- **多重安全**：NFC+蓝牙双重认证机制可选
- **拓展性强**：接口友好，可追加GPS、能耗统计等功能

## 目录结构
- `docs/` 设计方案、协议、MVP说明等文档
- `firmware/` ESP32主板固件代码，包括NFC、BLE、继电器等逻辑
- `app/` 手机App基础实现（Flutter推荐）
- `hardware/` 接线图、PCB、元件清单

## 快速启动
1. 按 [docs/hardware.md](docs/hardware.md) 接好硬件
2. 烧录 [firmware/main.ino](firmware/main.ino) 到ESP32
3. 使用 `app/` 目录下App试用核心功能

## 主要依赖
- ESP32 Arduino/ESP-IDF
- PN532 NFC模块
- Flutter（安卓/iOS App）

详细开发和扩展请参考 `docs/` 子目录下相关文档。