<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=280&section=header&text=XiNian-dada&fontSize=50&lineHeight=78&fontAlign=50&animation=fadeIn&fontColor=ffffff&desc=Bridging%20Silicon%20%26%20Software%20%7C%20Systems%2C%20Embedded%20%26%20Hardware&descAlign=50&descSize=16&descMarginTop=24" alt="header" />

> **「软硬兼施，探寻底层与现实的交界」**  
> _Bridging silicon and software — building low-level, high-impact systems from logic gates to distributed services._

<br/>

</div>

---

## About Me

你好，我是 **XiNian_dada**。

我是一名专注于 **软硬件协同、嵌入式系统与底层系统级工程（Systems & Embedded Engineering）** 的开发者。

我不拘泥于单一技术栈或练习型项目，注重 **自下而上建立对计算系统的全景掌控** —— 从数字逻辑与芯片引脚，到操作系统内核接口、网络流控协议，再到现代跨平台高性能服务。主张 **从真实痛点出发、软硬兼施、有需求就写、有问题就修**。

### 核心关注与实践领域

* **嵌入式系统与硬件原型**  
  基于 ARM Linux 单板计算机（如 RK3399）与 MCU（ESP32 / STM32）进行外设驱动开发与软硬件联调。涉足 Linux 设备树配置（DTC）、USB Gadget（OTG 虚拟键鼠/介质）、V4L2 视频采集、电路隔离控制，以及使用 Bambu Lab 3D 打印进行物理外壳与结构设计。

* **系统级编程与交叉编译体系**  
  以现代 Rust 与 C/C++ 为核心，打磨兼具高并发与极低系统开销的系统守护进程、中间件与监控探针。深度运用 `cross` 与 `musl-cross` 针对 `aarch64-unknown-linux-musl` 等架构进行静态分发，结合 `cargo-miri` 验证底层内存安全与未定义行为。

* **网络基础设施、固件与协议分析**  
  针对 OpenWrt 路由器固件进行系统级定制与流量重定向（nftables / WireGuard / LuCI）。熟练使用 Wireshark 进行抓包逆向与协议分析，结合 Tailscale 搭建边缘与开发环境的异地互联。

* **端侧计算与底层交互系统**  
  结合 Qt 6 / SDL 构建高响应性的桌面与硬件交互应用，探索基于 OpenCV、ONNX / OpenVINO 以及 llama.cpp 的端侧轻量化边缘推理管道。

---

## Featured Projects

| 项目 | 领域 / 架构层级 | 核心技术栈 | 简介与特性 |
| :--- | :--- | :--- | :--- |
| [**WingmanKVM**](https://github.com/XiNian-dada/WingmanKVM) | 软硬协同 / 边缘硬件 | `Rust` `ARM Linux` `V4L2` `USB-Gadget` `GPIO` | **运行在 ARM Linux 板卡上的网页 KVM**。整合 HDMI 视频采集、USB OTG 模拟复合键鼠与虚拟介质、GPIO 继电器硬件电源控制。 |
| [**NodeLite**](https://github.com/XiNian-dada/NodeLite) | 系统性能 / 集群监控 | `Rust` `Vue 3` `Systems` · **59 Stars** | **生产级极轻量集群监控系统**。Server-Agent 架构，服务端空载内存 <15MB，Agent <2MB，单机支撑 11 万+ 指标/秒的高吞吐实时流。 |
| [**Fuck_My_Shit_Mountain**](https://github.com/XiNian-dada/Fuck_My_Shit_Mountain) | 工程规范 / 静态审查 | `AI Code Audit` `Pragmatism` · **499 Stars** | **证据驱动的自动化代码审计工具**。直击工程代码质量痛点，输出严谨无情绪的技术审查报告，获开发者社区广泛认可。 |
| [**VanishMe**](https://github.com/XiNian-dada/VanishMe) | 客户端安全 / 隐私对抗 | `TypeScript` `Security` · **92 Stars** | **浏览器指纹伪装与深度防追踪扩展**。在底层动态拦截与改写 Canvas、WebGL、AudioContext 以及硬件设备指纹特征。 |
| [**luci-app-wloc**](https://github.com/XiNian-dada/luci-app-wloc) | 路由固件 / 网络流控 | `Go` `OpenWrt` `LuCI` `nftables` | **OpenWrt 固件网络层重写插件**。在嵌入式网关层精准拦截与重写 WLOC 响应，专为复杂分流与 Wi-Fi Calling 环境打造。 |
| [**SmartWatch_ESP32**](https://github.com/XiNian-dada/SmartWatch_ESP32) | 微控制器 / 智能硬件 | `C++` `ESP32` `IoT` `Python` | **ESP32 生理体征监测与智能原型**。包含传感器底层脉搏采集固件，以及基于串口的实时高帧率波形监控仪表盘。 |

---

## 100 Libraries Challenge

我在进行一个长期的个人挑战：

> **三年内完成 100 个真正可用的开源项目与代码库**

每个项目都遵循三个基本原则：
1. **真实可用**：解决具体真实的工程场景或个人需求，不做半成品 Demo。
2. **文档自洽**：开箱即用，具备详尽的部署或接入说明。
3. **软硬结合**：既有底层硬件的控制驱动，也有现代系统级架构的打磨。

<div align="center">

| 目标 | 仓库 | 当前进度 |
|:---:|:---:|:---:|
| 100 Libraries | [XiNian-dada/100-libs-challenge](https://github.com/XiNian-dada/100-libs-challenge) | **63 / 100** |

</div>

---

## Technical Landscape

### 硬件、电路与物理实现 (Hardware, Circuits & Physical Prototyping)
- **Platforms**: ARM Linux SBC (FireFly RK3399, etc.), ESP32 (Wi-Fi/BLE), STM32 (ARM Cortex-M), Arduino
- **Low-Level Subsystems**: USB Gadget / UDC, V4L2 (Video4Linux), GPIO / 继电器隔离, I2C, SPI, UART
- **Hardware Prototyping**: Bambu Lab 3D Printing (结构件与外壳成型), 3D CAD Modeling
- **Digital Logic & Architecture**: Logisim-evolution (数字电路与 CPU 仿真), QEMU ARM 系统级仿真

### 系统级开发与工具链 (Systems Programming & Toolchains)
- **Core Languages**: Rust (2024 Edition), Modern C / C++, Go
- **Cross-Compilation & Build**: `cross`, `musl-cross` (针对 aarch64 musl 静态二进制分发), CMake, Ninja, vcpkg
- **Security & Analysis**: `cargo-miri` (未定义行为/内存安全验证), `cargo-audit`, `cargo-deny`
- **Application & UI Frameworks**: Qt 6 (Core, Quick3D, SerialPort, Network), SDL2 / SDL3, Swift (Native macOS)

### 网络、固件与安全工程 (Networking, Firmware & Security)
- **Firmware & Gateways**: OpenWrt (LuCI, 插件开发), Linux Kernel Networking (nftables, iptables)
- **Protocols & Tunnels**: WireGuard, Tailscale (Mesh VPN), WebSockets, ZeroMQ
- **Analysis & Testing**: Wireshark (协议解包与逆向分析), iperf3 (吞吐基准压测), NextTrace

### 端侧计算与全栈工具 (Edge Computing & Full-Stack)
- **Edge Inference & Vision**: OpenCV, ONNX Runtime, OpenVINO, llama.cpp / ggml
- **Systems & Containers**: Linux (Ubuntu, Debian, Alpine), Docker, Colima
- **Secondary Languages**: Python, TypeScript, Java

---

## Stats

<div align="center">
  <a href="https://github.com/XiNian-dada">
    <img src="https://github-stats-extended.vercel.app/api?username=XiNian-dada&show_icons=true&include_all_commits=true&theme=tokyonight&hide_border=true&cache_seconds=1800" height="160" alt="GitHub Stats" />
  </a>
  <a href="https://github.com/XiNian-dada">
    <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=XiNian-dada&layout=compact&theme=tokyonight&hide_border=true&cache_seconds=1800" height="160" alt="Top Languages" />
  </a>
</div>

---

<div align="center">

_Build things that actually get used — from silicon pins to distributed systems._

</div>
