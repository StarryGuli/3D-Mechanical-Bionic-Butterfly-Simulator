# 🦋 3D机械仿生蝴蝶仿真器 | 3D Mechanical Bionic Butterfly Simulator

> 基于曲柄摇杆机构参数计算与仿生翅膀运动可视化展示的交互式3D模拟器。  
> An interactive 3D simulator integrating crank-rocker mechanism parameter computation and bionic butterfly wing motion visualization.

---

## 🌐 在线体验 | Live Demo

👉 [点击这里体验网页版仿真器 | Try the simulator online](https://starryguli.github.io/3D-Mechanical-Bionic-Butterfly-Simulator/)

> 推荐使用 Chrome 或 Edge 浏览器。  
> Recommended browser: Chrome or Edge.

---

## 🎯 项目简介 | Overview

该项目将 **机械工程计算** 与 **仿生翅膀运动可视化** 有机结合，  
通过网页展示曲柄摇杆机构的实时运动与参数变化。  
用户可以调整机构参数、观察翅膀扇动、分析运动特性，  
是一款适合教学、研究与创意展示的交互式工具。

本项目基于初代项目 [**crank-rocker-calculator**](https://github.com/StarryGuli/crank-rocker-calculator) 改进而成，  
在原有四杆机构参数计算与动画求解的基础上，  
扩展了仿生蝴蝶双翼结构与三维联动渲染，  
实现了从平面计算工具到完整 **3D 仿生机械模拟平台** 的升级。

This project seamlessly integrates **mechanical engineering computation** with **bionic wing motion visualization**.  
It simulates a crank-rocker mechanism in real time on the web, allowing users to tweak linkage parameters,  
observe flapping motion, and analyze mechanical behavior — useful for education, research, and demonstration.

It is an evolution of the original [**crank-rocker-calculator**](https://github.com/StarryGuli/crank-rocker-calculator),  
enhancing it from a planar kinematic calculator into a **full 3D bionic simulation system**  
with dual-wing synchronization, real-time rendering, and mechanical linkage analysis.

---

## 🧩 系统组成 | System Components

### 🪶 1. 三维仿真环境 | 3D Simulation Scene

- 基于 **Three.js** 搭建，实现真实的三维机构动画；
    
- 模型包含曲柄、连杆、摇杆以及仿生翅膀；
    
- 支持鼠标左键旋转、右键平移、滚轮缩放；
    
- 可从任意角度观察蝴蝶翅膀运动姿态。
    

Built on **Three.js**, the 3D scene visualizes the mechanism in motion.  
The model includes crank, coupler, rocker, and bionic wings.  
Users can rotate, pan, and zoom using mouse controls to explore the flapping from any viewpoint.

---

### ⚙️ 2. 参数控制与显示 | Parameter Control & Display

- **左侧**：可调整四杆机构参数  
    （曲柄 _a_、连杆 _b_、摇杆 _c_、机架 _d_）；
    
- **右侧**：实时显示计算结果  
    包括 Grashof 判别、摆角、运动比 K、是否整周转动；
    
- 支持调整动画速度与机构夹角，模拟不同翅膀张合姿态。
    
- **Left side:** adjust the four-bar linkage parameters  
    (crank _a_, coupler _b_, rocker _c_, frame _d_);
    
- **Right side:** real-time display of computed results  
    including Grashof classification, swing amplitude, ratio _K_, and full rotation status;
    
- You can also control animation speed and linkage offset to simulate wing opening/closing.
    

---

### 🧠 3. 运动学计算引擎 | Kinematic Computation Engine

- 内置 Grashof 判别和几何约束求解算法；
    
- 支持反向求解设计：清空某一杆长并输入目标运动参数，系统自动解出该杆长；
    
- 所有计算均在客户端实时完成，无需刷新。
    
- Includes built-in Grashof condition evaluation and geometric solvers;
    
- Supports reverse-design: leave one linkage length blank and input a target motion,  
    then the system computes that missing length;
    
- All calculations run in real time on the client side — no page reload needed.
    

---

## 🧠 参数说明 | Parameter Description

|参数|Symbol|含义|Meaning|单位|
|---|---|---|---|---|
|曲柄长度|a|曲柄的长度|Crank length|mm|
|连杆长度|b|连杆的长度|Coupler length|mm|
|摇杆长度|c|摇杆的长度|Rocker length|mm|
|机架长度|d|机架的长度|Frame length|mm|
|机构系数|K|运动比|Motion ratio|—|
|摆角|θ|摇杆摆动幅度|Swing amplitude|°|

---

## 🧰 技术栈 | Tech Stack

|技术|描述|Technology|Description|
|---|---|---|---|
|**Three.js**|三维渲染引擎|3D rendering library|For visualizing and animating 3D models|
|**JavaScript (ES6)**|运动学计算与动画控制|Parametric logic & animation|Core logic & real-time updates|
|**HTML + CSS**|用户界面布局与样式|UI & styling|Front-end presentation and inputs|

---

## 🚀 快速运行 | Quick Start

### 本地运行 | Run Locally

```bash
git clone https://github.com/starryguli/3D-Mechanical-Bionic-Butterfly-Simulator.git
cd 3D-Mechanical-Bionic-Butterfly-Simulator 
open index.html
```