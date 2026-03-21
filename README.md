# SpharxWorks 数据智能基础设施

<div align="center">

[![License](https://img.shields.io/badge/license-GPL3.0-blue.svg)](LICENSE)
[![AgentOS License](https://img.shields.io/badge/AgentOS-Apache2.0-green.svg)](AgentOS/LICENSE)
[![Python](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![C/C++](https://img.shields.io/badge/C%2FC%2B%2B-11%2F17-blue.svg?logo=c%2B%2B&logoColor=white)](https://isocpp.org/)
[![Docker](https://img.shields.io/badge/docker-ready-green.svg)](https://www.docker.com/)
[![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20Windows-lightgrey.svg)](#)


**人工智能时代的物理世界数据基础设施**
-

<h4>“From data intelligence emerges”<h4>
<h4>“始于数据，终于智能”<h4>

</div>

## 🎯 项目愿景

- **SPHARX极光感知**：成为人工智能时代的"数据台积电"。
- **四位一体架构**：数据采集 (Workshop) + 深度加工 (Deepness) + 评测验证 (Benchmark) + 智能体运行时 (AgentOS)
- **工业化生产理念**：通过标准化、模块化的生产体系，构建从物理世界到数字智能的完整基础设施。
- **我们相信**：真正的智能源于对物理世界的深度理解和精准建模，终于自主决策与执行。

---

## 🏭 核心价值

### 工业化生产体系
- **标准化**：从数据采集到模型训练的端到端标准化流水线
- **模块化**：可插拔的处理模块，支持灵活扩展和定制
- **质量保障**：贯穿全流程的自动化质检和数据完整性验证
- **规模效应**：通过平台化运营实现边际成本递减

### 平台化生态
- **开放标准**：建立物理世界数据的行业标准和规范
- **生态协同**：连接硬件厂商、算法开发者和应用企业
- **价值共创**：构建多方共赢的数据价值网络
- **持续进化**：基于反馈循环的智能化升级机制

### 智能体操作系统
- **微内核架构**：最小化内核设计，所有服务运行在用户态
- **三层一体**：认知层、行动层、记忆层协同工作
- **记忆卷载系统**：L1-L4 渐进式记忆抽象，支持存储、检索、进化和遗忘
- **系统调用抽象**：稳定安全的系统调用接口，隐藏内核实现细节
- **多语言 SDK**：Go、Python、Rust、TypeScript 原生支持

---

## 🚀 四大核心子系统

SpharxWorks 采用分层架构设计，包含四条核心产品线，分别负责数据采集预处理、深度加工、评测验证和智能体运行时：



## 🤖 1. AgentOS - 智能体超级操作系统 ✅ 生产就绪 (v1.0.0.5)

AgentOS（SuperAI OS）是 SpharxWorks 的核心智能体操作系统内核，提供完整的智能体运行时环境、记忆系统、认知引擎和执行框架。作为物理世界数据基础设施的生产级操作团队，AgentOS 实现了从数据处理到智能决策的完整闭环。

### 🎯 核心价值

- **微内核**: 最小化内核设计，所有服务运行在用户态，确保系统稳定性和可扩展性
- **三层一体架构**: 认知层、行动层、记忆层协同工作，实现智能体完整生命周期管理
- **记忆卷载系统**: L1-L4 渐进式记忆抽象，支持记忆存储、检索、进化和遗忘
- **系统调用抽象**: 稳定安全的系统调用接口，隐藏内核实现细节
- **可插拔策略**: 认知、规划、调度等核心算法支持动态加载和运行时替换
- **统一日志系统**: 跨语言日志接口，支持全链路追踪和 OpenTelemetry 集成
- **多语言 SDK**: Go、Python、Rust、TypeScript 原生支持，FFI 接口高效安全

### 📊 版本状态

**当前版本**: v1.0.0.5 (生产就绪 | 完成度：85%)

- ✅ **MemoryRovol 记忆卷载系统**
  - L1-L4 四层架构全部实现
  - 同步/异步写入支持（10,000+ 条/秒）
  - FAISS 向量检索集成（IVF/HNSW 索引）
  - 吸引子网络检索机制
  - 艾宾浩斯遗忘曲线实现
  - LRU 缓存与向量持久化
- ✅ **CoreLoopThree 三层一体架构**
  - 认知层：意图理解、任务规划、多策略协同（90%）
  - 行动层：执行引擎、补偿事务、责任链追踪（85%）
  - 记忆层：MemoryRovol FFI 封装（80%）
- ✅ **微内核基础模块 (core)** 实现
  - IPC Binder 通信
  - 内存管理（RAII、智能指针）
  - 任务调度（加权轮询）
  - 高精度时间服务
- ✅ **系统调用层 (syscall)** 开发完成 (100%)
  - ✅ 任务系统调用：`sys_task_submit/query/wait/cancel`
  - ✅ 记忆系统调用：`sys_memory_write/search/get/delete`
  - ✅ 会话系统调用：`sys_session_create/get/close/list`
  - ✅ 可观测性调用：`sys_telemetry_metrics/traces`
  - ✅ 统一入口：`agentos_syscall_invoke()`
- 🔲 完整端到端集成测试

### 🏗️ 系统架构

**详见**: [CoreLoopThree 架构详解](AgentOS/partdocs/architecture/coreloopthree.md)

### 💾 MemoryRovol: 四层记忆卷载系统

**核心功能**:
- **记忆存储**: 同步/异步写入，10,000+ 条/秒吞吐
- **记忆检索**: FAISS 向量检索 (<10ms)，混合检索，重排序
- **记忆进化**: L1→L2→L3→L4 渐进式抽象
- **记忆遗忘**: 艾宾浩斯曲线，自动遗忘任务

**详见**: [MemoryRovol 架构详解](AgentOS/partdocs/architecture/memoryrovol.md)

### 🛠️ 快速开始

```bash
# 克隆项目
git clone https://gitee.com/spharx/agentos.git
cd agentos

# 构建
cmake ../atoms -DCMAKE_BUILD_TYPE=Release -DBUILD_TESTS=ON
cmake --build . --parallel $(nproc)

# 测试
ctest --output-on-failure
```

**开发指南**: [AgentOS 开发文档](AgentOS/partdocs/guides/getting_started.md)

---

## 🏭 2. Workshop - 物理世界数据工厂 ✅ 生产就绪 (v1.0.3.7)

Workshop 是 SpharxWorks 的数据采集与预处理核心平台，采用模块化、容器化的架构设计，实现了从原始传感器数据到标准化高质量数据集的完整处理链路。作为物理世界数据工厂，为后续的深度加工提供高质量的数据基础。

### 🔄 完整处理链路

Workshop 采用六阶段流水线处理架构，每个模块承担特定职责：

```
原始数据输入 
→ 00_ingest 
→ 01_quality 
→ 02_enhance 
→ 03_calibrate 
→ 04_pack 
→ 05_delivery 
→ 标准化数据集
```

### 🧩 核心模块详解

#### 00_ingest - 数据导入模块
- **功能职责**：接收和解析原始传感器数据，实现隐私脱敏处理
- **技术栈**：Intel RealSense SDK、OpenCV、ROS Bag 解析
- **输入格式**：ROS Bag 文件、RealSense 数据流
- **输出结构**：标准化目录结构（rgb/、depth/、calibration/、timestamps.csv等）
- **关键技术**：实时数据流处理、隐私保护算法

#### 01_quality - 质量检测模块
- **功能职责**：多层次数据质量评估与验证
- **检测维度**：硬件层（模糊度、曝光、帧率）、语义层（动作完整性）
- **输出产物**：quality_report.json、详细质量指标数据
- **配置灵活性**：可调节的质量阈值和检测参数

#### 02_enhance - 数据增强模块
- **功能职责**：基于目标检测的数据增强和自动标注
- **核心技术**：YOLOv8 实时目标检测、图像去噪算法
- **输出格式**：COCO 格式标注文件、增强后的图像数据
- **模型支持**：yolov8n.pt（可替换为其他 YOLOv8 模型）

#### 03_calibrate - 相机标定模块
- **功能职责**：相机内外参精确标定
- **标定方法**：棋盘格标定法、标定精度验证
- **输出内容**：内参矩阵、外参矩阵、详细标定报告
- **支持范围**：单相机内参标定（外参标定预留）

#### 04_pack - 数据打包模块
- **功能职责**：标准化数据集打包与完整性校验
- **支持格式**：ROS Bag 格式、COCO 格式、自定义扩展格式
- **质量保证**：自动完整性检查、SHA256 校验和生成
- **验证机制**：格式验证和数据一致性检查

#### 05_delivery - 数据交付模块
- **功能职责**：数据集上传和交付管理
- **交付方式**：阿里云 OSS 对象存储、SFTP 安全传输、本地存储
- **可靠性保障**：重试机制、交付状态通知、完整性验证

### 🛠️ 技术架构

**基础设施**：
- **容器化**：基于 Docker 的微服务架构，支持弹性扩展
- **编程语言**：Python 3.10+，核心框架包括 OpenCV、PyTorch、YOLOv8
- **硬件支持**：Intel RealSense SDK，支持多种传感器设备
- **配置管理**：YAML 格式统一配置，环境变量灵活控制

**工程实践**：
- **配置驱动**：模块化配置管理体系，支持热更新
- **监控可观**：完善的日志系统和实时状态监控
- **安全合规**：容器安全策略和数据保护机制
- **持续集成**：自动化测试和部署流水线

### 📈 当前应用状况

Workshop v1.0.3.7 版本已达到生产就绪状态，在实际项目中稳定运行：
- ✅ 完成硬件同步方案（3×D455 相机）
- ✅ 实现 RealSense 数据解析功能
- ✅ 集成 YOLOv8 目标检测
- ✅ 建立完整的质量控制体系
- ✅ 支持多种数据交付方式
- ✅ 六阶段流水线全部模块生产就绪

**文档**: [Workshop 完整文档](Workshop/README.md) | [架构设计](Workshop/docs/WORKSHOP_ARCH.md)

---

## ⚡ 3. Deepness - 深度加工生产线 ⚡ 开发中 (v1.0.4.0)

Deepness 是 SpharxWorks 的核心深度加工子系统，致力于将原始物理世界数据转化为富含语义和物理属性的高价值数据资产。系统采用模块化、容器化的设计理念，通过四个核心处理管道实现从基础数据到高级应用的完整转换链路。

### 🎯 核心价值

- **物理世界数字化**：将现实场景转化为可计算、可仿真的数字孪生体
- **语义丰富化**：为3D场景注入丰富的语义和物理属性信息
- **交互建模**：记录和分析物理交互行为，支持反事实推演
- **标准输出**：生成符合主流评测框架的标准化数据格式

### 🔄 四大核心处理管道

#### 01_spatial_prior - 空间先验生成管道
- **技术基础**: 基于 NVIDIA Cosmos 世界模型实现空间理解
- **核心功能**: 生成场景的语义分割和几何先验
- **输出产物**: 语义地图、几何先验、Cosmos 特征向量
- **技术栈**: PyTorch 2.5.1 (CUDA 12.1)、NVIDIA Cosmos

#### 02_physics_jepa - 物理属性预测管道
- **技术基础**: 基于 Meta JEPA 架构预测物体物理属性
- **核心功能**: 推断材质、密度、摩擦系数等参数
- **输出产物**: 标准化 3D 网格模型、物理属性元数据
- **技术栈**: PyTorch 2.5.1、PyTorch3D 0.7.6、Open3D 0.18.0

#### 03_causal_trajectory - 交互轨迹记录管道
- **技术组成**: 整合多模态感知数据（RGB-D + IMU）
- **核心能力**: 记录物理交互轨迹和行为模式
- **高级功能**: 支持反事实推演和仿真验证
- **技术支撑**: YOLOv8 目标检测、ORB-SLAM3/LIO-SAM 定位、PyBullet 物理仿真

#### 04_benchmark_export - 评测数据导出管道
- **转换能力**: 支持多种标准评测格式
- **兼容框架**: Genie Sim 3.0、NVIDIA Cosmos、Meta JEPA 等主流框架
- **质量保障**: 提供数据质量报告和完整性验证
- **扩展支持**: 可定制的导出适配器

### 📊 技术架构详情

**基础设施**:
- **Docker 容器化**: 基于 CUDA 12.1 的 Ubuntu 22.04 基础镜像
- **Python 环境**: Miniforge3 + Python 3.11，预装科学计算包
- **深度学习**: PyTorch 2.5.1 (CUDA 12.1)、PyTorch3D 0.7.6
- **3D 处理**: Open3D 0.18.0、Kaolin 0.17.0、gsplat 渲染引擎
- **世界模型**: NVIDIA Cosmos、Meta JEPA
- **视觉算法**: YOLOv8、ORB-SLAM3、LIO-SAM

**配置管理**:
- **统一配置中心**: YAML 格式，支持模块化配置
- **环境变量控制**: 通过 .env 文件管理运行参数
- **版本锁定**: deps.lock 文件确保依赖一致性

### 📈 开发进度与规划

当前版本 v1.0.4.0 开发进度 80%:
- ✅ 基础架构搭建完成
- ✅ Docker 容器化配置就绪
- ✅ 四个核心处理模块全部实现
  - ✅ run_01_spatial_prior (Cosmos 适配器)
  - ✅ run_02_physics_jepa (JEPA 物理预测)
  - ✅ run_03_causal_trajectory (SLAM+ 因果推理)
  - ✅ run_04_benchmark_export (多格式导出)
- ⏳ 端到端集成测试中 (80%)
- 🔲 性能基准测试

**文档**: [Deepness 技术文档](Deepness/README.md) | [管道详解](Deepness/docs/README_pipelines.md)

---

## 📊 4. Benchmark - 世界模型评测中心 📊 规划中 (v1.0.0.1)

Benchmark 是 SpharxWorks 的世界模型评测中心，旨在建立标准化的世界模型评估体系，推动物理AI领域的健康发展。该系统将提供权威的评测基准、标准化的数据集和科学的评估指标。

### 🎯 系统愿景

- **标准化评估体系**：建立统一的世界模型评测标准
- **多维度评测框架**：支持物理理解、交互预测、场景重建等多个维度
- **开放包容生态**：兼容主流评测框架，促进技术交流与发展
- **持续进化机制**：基于社区反馈不断优化评测标准

### 🏗️ 核心功能规划

#### 标准数据集管理
- **多样化场景**：涵盖室内、室外、工业等多种应用场景
- **质量保证**：严格的数据采集和标注标准
- **版本控制**：完善的版本管理和更新机制
- **开放获取**：支持学术研究和商业应用

#### 评测框架集成
- **主流框架支持**: Genie Sim 3.0、NVIDIA Cosmos、Meta JEPA 等
- **自定义适配器**: 支持第三方评测框架集成
- **自动化评测**: 一键式评测流程，降低使用门槛
- **结果可视化**: 直观的评测报告和性能分析

#### 指标体系建设
- **基础性能指标**：准确率、召回率、F1分数等
- **物理合理性**：物理属性预测准确性
- **交互智能度**：交互行为预测能力
- **泛化能力**：跨场景适应性评估

### 🔧 技术架构设计

**系统架构**：
- **微服务设计**：模块化架构，支持独立扩展
- **容器化部署**：基于 Docker 的弹性部署方案
- **API 接口**：标准化 RESTful API，支持第三方集成
- **数据存储**：分布式存储，确保数据安全可靠

**开发技术栈**：
- **后端框架**：Python FastAPI/Flask
- **前端界面**：React/Vue.js 现代化界面
- **数据库**：PostgreSQL + Redis 缓存
- **消息队列**：RabbitMQ/Kafka 异步处理

### 📈 当前状态与规划

当前版本 v1.0.0.1 处于架构设计阶段（25% 完成）:
- 🔲 需求分析和系统设计
- 🔲 技术选型和架构确定
- 🔲 核心模块原型开发
- 🔲 评测标准制定

**发展路线图**:
- v1.0.0.1 - 架构设计和原型验证
- v1.0.1 - 基础评测功能实现
- v1.1.0 - 多框架集成和标准发布
- v2.0.0 - 智能化评测和生态完善

**文档**: [Benchmark 设计文档](Benchmark/metrics/README.md)

---

## 📈 整体发展路线图

### 短期目标 (2026 Q2-Q3)
- ✅ **Workshop v1.0.3.7** 生产就绪 - 六阶段流水线全部模块完成
- ⏳ **Deepness v1.0.4.0** 端到端集成 (80%) - 四大处理管道联调中
- ⏳ **AgentOS v1.0.0.5** 核心实现 (85%) - CoreLoopThree/MemoryRovol/系统调用完成
- 🔲 **Benchmark v1.0.0.1** 架构设计 (25%) - 需求分析和原型验证

### 中期规划 (2026 Q4-2027)
- 🚀 **Deepness v1.1.0** 正式发布 - 完成性能基准测试和生产部署
- 🚀 **AgentOS v1.1.0** 生产就绪 - 完整 SDK、多智能体协同、高级认知功能
- 📊 **Benchmark v1.0.1** 基础评测功能 - 标准数据集管理和自动化评测流程
- 🔄 **四大系统协同生态** - Workshop→Deepness→Benchmark→AgentOS 完整数据流
- 🌐 **开发者生态** - Go/Python/Rust/TypeScript 多语言 SDK 完善

### 长期愿景 (2027+)
- 🌐 **物理 AI + 智能体 OS 双轮驱动** - 成为人工智能时代的数据基础设施
- 🤝 **全球化开源社区** - 建立开放包容的技术生态
- 🏆 **下一代技术引领** - 物理世界理解与智能决策技术的持续创新
- 📈 **Benchmark v2.0.0** 智能化评测 - 自适应评估和进化能力
- 🤖 **AgentOS v2.0.0** 通用人工智能操作系统 - 支持 AGI 级智能体运行时

---

## 🤝 生态合作

我们诚邀各界合作伙伴共同建设物理世界数据基础设施与智能体操作系统生态：

### 技术合作伙伴
- **硬件厂商**：传感器、相机、GPU/NPU计算设备提供商
- **算法团队**：3D 重建、SLAM、物理仿真、大模型、认知架构等领域专家
- **应用企业**：机器人、自动驾驶、AR/VR、智能助理等落地场景

### 社区贡献
- **代码贡献**：核心功能开发和优化
- **文档完善**：使用指南和技术文档
- **测试验证**：功能测试和性能评估
- **生态建设**：社区运营和知识分享

---

## 📧 联系方式

### 统一联系邮箱
- **技术支持**：lidecheng@spharx.cn（Workshop / Deepness / Benchmark）
- **安全问题**：wangliren@spharx.cn（安全漏洞报告）
- **商务合作**：zhouzhixian@spharx.cn

### 官方网站
- **主站**：https://spharx.cn
- **Gitee 仓库**：https://gitee.com/spharx
- **GitHub 镜像**：https://github.com/SpharxTeam

## 📚 技术资源

### 核心文档
- [🤖 **AgentOS 完整文档**](AgentOS/README.md) - 智能体操作系统详细说明 ⭐ 新增
- [📘 **Workshop 完整文档**](Workshop/README.md) - 数据工厂详细说明
- [🔬 **Deepness 技术文档**](Deepness/README.md) - 深度加工技术细节
- [📊 **Benchmark 设计文档**](Benchmark/metrics/README.md) - 评测系统规划

### 架构设计
- [🧠 **CoreLoopThree 架构**](AgentOS/partdocs/architecture/coreloopthree.md) - AgentOS 三层一体核心运行时 ⭐ 新增
- [💾 **MemoryRovol 架构**](AgentOS/partdocs/architecture/memoryrovol.md) - AgentOS 四层记忆卷载系统 ⭐ 新增
- [🏗️ **Workshop 架构文档**](Workshop/docs/WORKSHOP_ARCH.md) - 详细架构设计
- [🔬 **Deepness 管道文档**](Deepness/docs/README_pipelines.md) - 处理管道详细说明
- [📊 **Benchmark 架构文档**](Benchmark/metrics/README.md) - 评测系统架构（规划中）

### 开发资源
- [🚀 **AgentOS 开发指南**](AgentOS/partdocs/guides/getting_started.md) - 快速开始和开发教程
- [📋 **编码规范**](Workshop/docs/CODING_STANDARDS.md) - 开发标准和规范
- [🧪 **测试指南**](Workshop/tests/docs/TESTING_GUIDE.md) - 测试框架说明
- [📈 **项目进度**](Workshop/docs/PROGRESS.md) - 开发里程碑跟踪

---

## 📄 许可证与授权

### SpharxWorks 整体许可证（适用于 Workshop / Deepness / Benchmark）

SpharxWorks 采用 **GPL-3.0 开源协议 + 商业闭源授权** 双授权模式，您可根据自身使用场景选择对应授权。

#### 开源授权（GPL-3.0）
个人学习、学术研究、非商业原型验证、开源社区贡献等非商业场景，可免费使用本项目，需严格遵守 GPL-3.0 协议的开源义务，完整协议详见 [LICENSE-GPL-3.0](LICENSE-GPL-3.0)。

#### 商业闭源授权
任何将本项目用于闭源商业产品、商业服务、盈利性项目的行为，均需提前向 SPHARX 极光感知科技申请商业授权，获得闭源使用豁免、官方技术支持、定制化服务等权益。

商业授权详情详见 [LICENSE-COMMERCIAL](LICENSE-COMMERCIAL)，授权申请请联系：
- 官方邮箱：lidecheng@spharx.cn、wangliren@spharx.cn
- 官方网站：https://spharx.cn

---

### AgentOS 分层许可证

AgentOS 作为智能体操作系统，采用更加灵活的**分层开源协议**:

| 模块 | 许可证 | 说明 |
|------|--------|------|
| **atoms/** (微内核基础) | Apache License 2.0 | 核心内核模块，允许商业集成 |
| **domes/** (CoreLoopThree/MemoryRovol) | Apache License 2.0 | 核心运行时和记忆系统 |
| **openhub/** (应用层) | MIT License | 示例应用和 SDK，极度宽松 |
| **第三方依赖** | 原协议 | 遵循各自开源协议 |


完整协议详见 [AgentOS LICENSE](AgentOS/LICENSE)。

---

## 🙏 致谢

感谢所有为开源社区做出贡献的开发者们，正是你们的努力让这样的项目成为可能。



<div align="center">

<h3>From data intelligence emerges</h3>
<h3>始于数据，终于智能</h3>

<p><em>构建 AI 时代的物理世界数据基础设施与智能体操作系统</em></p>

#### 📞 联系我们

📧 邮箱：lidecheng@spharx.cn & wangliren@spharx.cn

<p>
  <a href="https://github.com/spharx">GitHub</a> ·
  <a href="https://gitee.com/SpharxTeam">Gitee</a> ·
  <a href="https://spharx.cn">官方网站</a> ·
  <a href="mailto:lidecheng@spharx.cn">技术支持</a>
</p>

© 2026 SPHARX Ltd. All Rights Reserved.

</div>