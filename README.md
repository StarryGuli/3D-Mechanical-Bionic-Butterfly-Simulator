# 🦋 3D机械仿生蝴蝶仿真器 | 3D Mechanical Bionic Butterfly Simulator

> 基于曲柄摇杆机构参数计算与仿生翅膀运动可视化展示的交互式3D模拟器。  
> An interactive 3D simulator integrating crank-rocker mechanism parameter computation and bionic butterfly wing motion visualization.

---

## 🌐 在线体验 | Live Demo

👉 [点击这里体验网页版仿真器（GitHub Pages）](https://yourusername.github.io/3D-Mechanical-Bionic-Butterfly-Simulator/)  
> 支持桌面端浏览器（推荐 Chrome / Edge），可自由旋转、缩放与参数调节。

---

## 🎯 项目简介 | Overview

这是一个基于网页的三维交互式仿真平台，  
将 **机械工程计算** 与 **仿生翅膀运动可视化** 相结合，  
可用于教学、研究或创意展示。

- **实时可视化**：以三维动画展示曲柄摇杆机构的真实运动。
- **参数计算**：内置 Grashof 判别、摆角、K 系数与整周判断。
- **反推设计**：支持输入目标运动参数，自动反解杆长。
- **交互控制**：通过滑块与鼠标操作调整姿态、速度与角度。
- **轻量运行**：纯前端 WebGL 实现，无需服务器环境。

---

## 🧩 系统结构 | System Structure

### 🪶 1. 三维仿真环境
- 基于 **Three.js** 构建 3D 场景；
- 模型包含连杆、铰接点与仿生翅膀；
- 支持鼠标拖拽旋转、滚轮缩放和平移操作。

### ⚙️ 2. 参数控制与计算
- 左侧：调节曲柄 (a)、连杆 (b)、摇杆 (c)、机架 (d)；
- 右侧：实时显示机构判别、摆角、系数 K、整周转动结果；
- 可调整动画速度与机构夹角，模拟不同翅膀张开姿态。

### 🧠 3. 运动学引擎
- 内置四杆机构运动学分析算法；
- 自动判别 Grashof 条件；
- 支持反向求解与动态更新；
- 完全使用 JavaScript 实时运算。

---

## 🧠 参数含义 | Parameters

| 参数 | 符号 | 含义 | 单位 |
|------|------|------|------|
| 曲柄长度 | a | crank length | mm |
| 连杆长度 | b | coupler length | mm |
| 摇杆长度 | c | rocker length | mm |
| 机架长度 | d | frame length | mm |
| 机构系数 | K | motion ratio | - |
| 摇杆摆角 | θ | swing amplitude | ° |

---

## 🧰 技术栈 | Tech Stack

- **Three.js** — 3D 图形渲染  
- **JavaScript** — 参数计算与动画控制  
- **HTML + CSS** — 界面与布局  

---

## 🚀 快速运行 | Quick Start

1. 克隆项目：
   ```bash
   git clone https://github.com/yourusername/3D-Mechanical-Bionic-Butterfly-Simulator.git
