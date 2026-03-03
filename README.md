数据资产管理平台原型
项目简介

本项目为数据资产管理平台的原型系统，基于HTML构建前端界面，集成数据资产全生命周期管理核心功能，涵盖资产盘点、分级分类、标准管理、目录元数据、质量监控、可视化分析等模块，旨在为企业提供数据资产的规范化管理与高效利用支持。原型版本为 v1.0.0，包含完整功能演示文件与交互逻辑。

核心功能模块
1. 数据资产盘点

支持盘点任务创建、执行与监控（含定时任务配置），提供任务列表（名称、数据源、执行状态、创建人等）及操作（查看/复制/删除）。

关联“数据资产盘点任务执行列表”“配置盘点任务”“详情-盘点结果确认”等子功能，覆盖从任务发起至结果核验全流程。

2. 分级分类管理

实现数据资产的分级（如敏感等级）与分类（如业务域、技术域）定义，支持多级目录（一级/二级/三级）管理。

提供“分级分类报告”生成与查询，辅助资产价值评估。

3. 数据标准与元数据管理

数据标准管理：定义数据业务标准、技术规范，支持“数据标准管理(暂定)”迭代。

目录元数据管理：包括初始页面配置、元数据扫描与监控（“详情-元数据扫描”“详情-元数据扫描监控”）、智能解析（“详情-数据智能解析监控”）等。

4. 资产目录与清单

资产目录列表/详情页：展示资产层级结构、关联关系（如“详情-数据关联分析”“详情-数据关联分析监控”）。

数据资产清单：整合库级/表格/字段级资产，支持多维度筛选与导出。

5. 数据资产应用与报告

数据资产应用：对接业务场景，提供API资产清单、标签资产清单等。

数据资产报告：自动生成资产总量、分布、热词（词云图）、Top10数据表/标签等统计报告，含可视化图表（环形图、柱状图、条形图）。

6. 基础支撑功能

数据源管理：接入多源数据，监控数据源状态。

数据质量管理：配置质量规则，监控异常数据。

用户权限：支持“用户权限”“权限管理”模块，保障资产安全。

系统架构与流程
1. 管理流程（参考数据资产管理流程图
，见第3张图）

角色：数据资产管理总体责任人、资产管理人员/组织、数据源责任人、数据开发责任人、资产使用者。

核心步骤：新库发现更新 → 数据分级分类 → 数据关联分析 → 开发/生产变更管理 → 数据资产稽核 → 资产使用与核验 → 总结通告。

2. 支撑体系

工具层：数据资产盘点工具、资产清单（标准/主数据/标签/API）、数据资产报告、标签管理。

制度层：数据资产管理制度、分级分类规范、质量标准、安全策略。

界面特点

导航设计：左侧深蓝色侧边栏，集成“分级分类管理”“数据资产盘点”“数据资产报告”等20+功能入口，当前操作高亮显示。

可视化分析：主内容区支持多图表联动，包括数据表IP分布环形图、数据类别分布圆环图、标签Top10柱状图、数据量Top10条形图、热词词云图。

任务管理：“盘点任务列表”页支持任务搜索、状态筛选，操作区提供“查看/复制/删除”快捷功能，蓝白主色调简洁直观。

快速开始

获取原型文件：下载仓库内 数据资产管理原型v1.0.0.zip，解压后直接打开HTML文件（如start.html）进入演示界面。

在线查看：访问 [GitHub Pages链接]（若已部署），或通过仓库“Preview”模式在线浏览文件内容。

功能体验：重点体验“分级分类管理.html”“数据资产盘点任务列表.html”“数据资产报告.html”等核心页面。

贡献指南

欢迎提交Issue反馈问题，或通过Pull Request贡献代码/优化建议。请确保修改符合数据资产管理领域最佳实践。

Data Asset Management Platform Prototype
Project Overview

This project is a prototype of a Data Asset Management Platform, built with HTML for the frontend. It integrates core functionalities for full-lifecycle data asset management, including inventory, classification & grading, standard management, metadata management, quality monitoring, and visualization analysis. The prototype version is v1.0.0, containing complete demo files and interaction logic.

Core Functional Modules
1. Data Asset Inventory

Supports inventory task creation, execution, and monitoring (including scheduled tasks), with a task list (name, data source, status, creator, etc.) and operations (view/copy/delete).

Links to sub-features like "Data Asset Inventory Task Execution List," "Configure Inventory Task," and "Details - Inventory Result Confirmation."

2. Classification and Grading Management

Implements data sensitivity grading and business/technical classification, supporting multi-level directories (1st/2nd/3rd level).

Generates and queries "Grading and Classification Reports" to assist in asset value assessment.

3. Data Standards and Metadata Management

Data Standards Management: Defines business/technical standards, supporting iterative updates (e.g., "Data Standard Management (Tentative)").

Catalog Metadata Management: Includes initial page configuration, metadata scanning/monitoring ("Details - Metadata Scanning"), and intelligent parsing ("Details - Intelligent Parsing Monitoring").

4. Asset Catalog and Inventory

Asset Catalog List/Details: Displays hierarchical structure and relationships (e.g., "Details - Data Correlation Analysis").

Data Asset Inventory: Integrates library/table/field-level assets with multi-dimensional filtering and export.

5. Data Asset Application and Reporting

Application: Connects to business scenarios, providing API/tag asset inventories.

Reporting: Auto-generates reports on total volume, distribution, hot keywords (word cloud), Top 10 tables/tags, with visualizations (donut charts, bar charts, line charts).

6. Basic Support Functions

Data Source Management: Accesses multi-source data and monitors source status.

Data Quality Management: Configures quality rules and monitors anomalies.

User Permissions: Manages access control via "User Permissions" and "Permission Management" modules.

System Architecture and Process
1. Management Process (Refer to Data Asset Management Flowchart
, see Screenshot 3)

Roles: Overall Responsible Person, Asset Managers/Organizations, Data Source Owners, Data Developers, Asset Users.

Key Steps: New Database Discovery/Update → Data Grading & Classification → Data Correlation Analysis → Development/Production Change Management → Asset Audit → Usage & Verification → Summary Notification.

2. Support System

Tool Layer: Inventory tools, asset inventories (standard/master data/tag/API), asset reports, tag management.

Policy Layer: Asset management policies, grading/classification norms, quality standards, security strategies.

Interface Features

Navigation: Dark-blue sidebar with 20+ entries (e.g., "Classification & Grading Management," "Data Asset Inventory"), highlighting current operations.

Visualization: Main content area supports multi-chart linkage: IP distribution donut chart, category distribution donut chart, Top 10 tags bar chart, Top 10 data volume bar chart, and hot keyword word cloud.

Task Management: "Inventory Task List" page enables search/filter by status, with quick operations (view/copy/delete) in a blue-white theme.

Quick Start

Get Prototype Files: Download 数据资产管理原型v1.0.0.zipfrom the repository, extract, and open HTML files (e.g., start.html).

Online Preview: Visit [GitHub Pages Link] (if deployed) or use the repository’s "Preview" mode.

Experience Features: Focus on core pages like "Classification and Grading Management.html," "Data Asset Inventory Task List.html," and "Data Asset Report.html."
