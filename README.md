# Perfect Cursor

> 🖱️ **Perfect Cursor** 是一个为 [Cursor](https://cursor.com) 打造的**最佳实践配置集合**。  
> 通过 **黄金标准文件（Gold-Standard Files）** + **反馈记忆机制（Feedback Memory Mechanism）**，  
> 让 AI 持续学习并产出更稳定、更高质量的代码。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Cursor Version](https://img.shields.io/badge/Cursor-Required-blue.svg)](https://cursor.com)
[![Documentation](https://img.shields.io/badge/Documentation-Complete-green.svg)](./CONFIGURATION_CN.md)
[![English](https://img.shields.io/badge/English-README_EN.md-blue.svg)](./README_EN.md)

简体中文 | [English](README_EN.md)

---

## ✨ 特性特性

- 🎯 **黄金标准文件** - 为 AI 设定质量标杆
- 🧠 **反馈记忆机制** - 让 AI 从错误中进化  
- 📚 **项目编码规范** - 统一的开发标准
- 🚀 **快速上手** - 简单易用的配置流程
- 🔧 **TypeScript 支持** - 完整的类型定义规范
- 🧪 **测试规范** - 统一的测试标准和流程
- 📝 **Git 工作流** - 标准化的版本控制流程

---

## 🚀 快速开始

### 前置要求

- [Cursor](https://cursor.com) 编辑器
- 基本的项目配置经验

### 安装配置

1. **克隆项目**
   ```bash
   git clone https://github.com/caterpi11ar/perfect-cursor.git
   cd perfect-cursor
   ```

2. **配置规则**
   - 在 `.cursor/rules/` 中添加或更新规则文件
   - 定期审查并更新黄金标准文件
   - 新增模块前，先参考黄金标准示例

3. **Code Review 时**
   - 将高频反馈沉淀到规则库

---

## 📁 项目结构

```
perfect-cursor/
├── .cursor/                    # Cursor 编辑器配置目录
│   └── rules/                  # 规则文件目录
│       ├── workflow.mdc        # 工作流规范
│       ├── project.mdc         # 项目开发规范
│       ├── typescript.mdc      # TypeScript 规范
│       ├── common.mdc          # 通用开发规范
│       ├── demo.mdc            # 演示代码规范
│       ├── git.mdc             # Git 工作流规范
│       └── testing.mdc         # 测试规范
├── README_EN.md                # 英文项目说明文档
├── CONFIGURATION_CN.md         # 中文配置说明文档
├── CONFIGURATION_EN.md         # 英文配置说明文档
└── ...                         # 其他项目文件
```

---

## 🔧 配置说明

### 黄金标准文件

**黄金标准文件**是精挑细选的**高质量代码示例**，它告诉 AI：
> "这是我们期望的风格与逻辑，请参考并保持一致。"

#### 创建与维护步骤

1. **精心选择示例**
   - **核心模块**：结构清晰、设计完善的核心业务模块
   - **通用组件**：API 设计优雅、被多处复用的 UI 组件或工具函数库
   - **典型页面**：包含数据获取、状态管理与交互逻辑的完整页面

2. **持续优化**
   - 每次重构或需求迭代后，更新这些文件
   - 文件可加特殊标记，方便团队与 AI 快速识别

3. **添加明确注解**
   - 在关键实现处，添加说明**为什么这么做**
   - 注释既能帮助新成员，也能为 AI 提供上下文参考

### 反馈记忆机制

**反馈记忆机制**将 Code Review 中反复出现的**共性问题**，沉淀为 AI 可直接理解的**规则文件**，减少重复性纠错。

#### 构建反馈记忆库

1. **创建规则目录**
   ```bash
   mkdir -p .cursor/rules
   ```

2. **将反馈转化为规则**
   - 每条常见反馈写成独立的 `.mdc` 文件
   - 文件名简明扼要
   - 规则描述应简洁、明确，可直接执行

---

## 📚 详细文档

- 📖 [配置说明](./CONFIGURATION_CN.md) - 详细的配置指南（中文）
- 📖 [Configuration Guide](./CONFIGURATION_EN.md) - Detailed configuration guide (English)
- 📋 [编码规范](./.cursor/rules/) - 项目编码规则
  - [工作流规范](./.cursor/rules/workflow.mdc)
  - [项目开发规范](./.cursor/rules/project.mdc)
  - [TypeScript 规范](./.cursor/rules/typescript.mdc)
  - [通用开发规范](./.cursor/rules/common.mdc)
  - [Git 工作流规范](./.cursor/rules/git.mdc)
  - [测试规范](./.cursor/rules/testing.mdc)

---

## 🎯 使用场景

- **团队开发** - 统一代码风格和开发规范
- **AI 辅助开发** - 通过规则文件指导 AI 生成优质代码
- **代码审查** - 减少重复性问题和提高审查效率
- **新人培训** - 快速了解项目开发规范和最佳实践
- **项目维护** - 保持代码质量和一致性

---

## ✅ 快速上手清单

* [ ] 在 `.cursor/rules/` 中添加或更新规则文件
* [ ] 定期审查并更新黄金标准文件
* [ ] 新增模块前，先参考黄金标准示例
* [ ] Code Review 时，将高频反馈沉淀到规则库
* [ ] 遵循 TypeScript 规范和 Git 工作流
* [ ] 按照测试规范编写测试用例

---

## 🤝 贡献指南

我们欢迎所有形式的贡献！请查看我们的 [贡献指南](.github/CONTRIBUTING.md) 了解详情。

### 贡献类型

- 🐛 报告 Bug
- 💡 提出新功能建议
- 📝 改进文档
- 🔧 提交代码修复
- 🧪 添加测试用例
- 📚 完善规则文件

### 贡献流程

1. Fork 项目
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

---

## 📄 许可证

本项目采用 [MIT 许可证](LICENSE) - 查看 [LICENSE](LICENSE) 文件了解详情。

---

## 🙏 致谢

感谢所有为这个项目做出贡献的开发者和用户！

特别感谢：
- [Cursor](https://cursor.com) 团队提供的优秀编辑器
- 所有贡献者和用户的支持与反馈

---

## 🌐 多语言支持

- 🇨🇳 [中文版](./README.md) - 当前页面
- 🇺🇸 [English Version](./README_EN.md) - 英文版本

---

<div align="center">
  <p>如果这个项目对你有帮助，请给它一个 ⭐️</p>
  <p>Made with ❤️ for the Cursor community</p>
</div>
